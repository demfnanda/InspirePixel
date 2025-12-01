<script setup>
    import card1 from "../assets/card1.png";
    import card2 from "../assets/card2.png";
    import card3 from "../assets/card3.png";
    import card4 from "../assets/card4.png";
    import card5 from "../assets/card5.png";
    import card6 from "../assets/card6.png";
    import card7 from "../assets/card7.png";
    import card8 from "../assets/card8.png";
    import card9 from "../assets/card9.png";
    import card10 from "../assets/card10.png";
    import card11 from "../assets/card11.png";
    import card12 from "../assets/card12.png";

    const cards = [
        card1, card2, card3, card4, card5, card6,
        card7, card8, card9, card10, card11, card12
    ]

</script>

<template>
    <section class="fotos">
        <h2>Inspire-se</h2>

        <div class="grid">

            <div
                v-for="(foto, index) in cards"
                :key="index"
                class="card"
                >
                <img :src="foto" alt="Foto" class="foto" />
            </div>

        </div>
  </section>
</template>



<style scoped lang="scss">

    .fotos {
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

            .card {
                img.foto {
                    width: 100%;
                    height: auto;
                    object-fit: cover;
                    border-radius: 16px;
                }
            }
    }

</style>