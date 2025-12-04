<script setup>
    const props = defineProps(["imagem"]);
</script>

<template>
    <div class="card">
        <img :src="props.imagem" alt="Imagem aleatória do Picsum" />
    </div>
</template>

<style scoped lang="scss">
    .card img {
        width: 100%;
        height: 100%;
        border-radius: 16px;
        aspect-ratio: 9 / 16;
        object-fit: cover;
    }
</style>