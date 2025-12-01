<script setup>
    import fotografo from "../assets/fotografo.png"
</script>

<template>

    <section class="banner">

        <div class="texto">

           <h1>Onde a paisagem vira 
             <span>inspiração</span> .
           </h1>
        
           <p>
             Exploque paisagens, cores e luzes que inspiram novas histórias através da fotografia.
           </p>

        </div>

        <div class="imagem">
            <img :src="fotografo" alt="">
        </div>
        
    </section>

</template>

<style scoped lang="scss">

    .banner{
        display: flex;
        align-items: center;
        justify-content: space-between;
        padding: 4rem 3rem;
        gap: 2rem;

        .texto{
            max-width: 50%;

            h1 {
                font-size: 3rem;
                font-weight: 800;
                color: #1d1d1d;
                line-height: 1.2;
                max-width: 500px;

                span {
                    color: #E1306C;
                }
            }

            p {
                margin-top: 1.5rem;
                font-size: 1.1rem;
                color: #262626;
                max-width: 600px;
                line-height: 1.5;
            }
        }

        .imagem{
            max-width: 45%;

            img {
                width: 100%;
                border-radius: 25px;
                object-fit: cover;
            }
        }
    }

</style>