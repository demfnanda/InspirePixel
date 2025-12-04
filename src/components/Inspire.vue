<script setup>
    import { ref, onMounted } from "vue";
    import axios from "axios";
    import Card from "./Card.vue";

    const imagens = ref([]);

    onMounted(async () => {
        try {
        const response = await axios.get("https://picsum.photos/v2/list?limit=12");
        imagens.value = response.data;
        } catch (error) {
        console.error("Erro ao buscar imagens:", error);
        }
    });
</script>

<template>

    <section class="inspire">
        <h2>Inspire-se</h2>

        <div class="grid">
            <Card
                v-for="img in imagens"
                :key="img.id"
                :imagem="img.download_url"
            />
        </div>
  </section>

</template>

<style scoped lang="scss">
    .inspire {
        padding: 2rem 3rem;

        h2 {
            font-size: 1.6rem;
            margin-bottom: 1.5rem;
            font-weight: 600;
        }

        .grid {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 1.5rem;
        }
    }

</style>