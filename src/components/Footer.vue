<script setup>
    import Facebook from "../assets/Facebook.png";
    import Linkedin from "../assets/Linkedin.png";
    import Instagram from "../assets/Instagram.png";
    import Twitter from "../assets/Twitter.png";
</script>

<template>
    <footer class="footer">

        <div class="footer-content">

            <section class="coluna1">
                <!-- Contato -->
                <div class="contato">
                    <h3>Contato</h3>
                    <p>contato@inspiralens.com</p>
                    <p>Central de ajuda</p>
                    <p>Rio de Janeiro – Brasil</p>
                </div>
            
                <!-- Sobre -->
                <div class="sobre">
                    <h3>Sobre</h3>
                    <p>Políticas</p>
                    <p>Políticas de privacidade</p>
                    <p>Blog</p>
             </div>
                
            </section>

            <section class="coluna2">
                <!-- Newsletter -->
                <div class="newsletter">
                 <h3>Assine nossa newsletter</h3>

                 <input
                 type="email"
                 placeholder="Seu e-mail"
                 />

                 <button>Inscrever-se</button>
             </div>

            </section>

            <!-- Ícones Sociais -->
             <div class="social">
                <img :src="Facebook" alt="Facebook" />
                <img :src="Linkedin" alt="LinkedIn" />
                <img :src="Instagram" alt="Instagram" />
                <img :src="Twitter" alt="Twitter" />
             </div>

        </div>

    </footer>

</template>

<style scoped lang="scss">
    .footer {
        padding: 4rem 2rem;
        background: #ffffff;


        .footer-content {
            display: flex;
            justify-content: space-between;
            flex-wrap: wrap;
            gap: 3rem;
        }


        h3 {
            font-size: 1.2rem;
            margin-bottom: 1rem;
            font-weight: 600;
        }


        p {
            margin: 0.4rem 0;
            color: #333;
        }


        .coluna1 {
            display: flex;
            gap: 4rem;
            margin-left: 1.8rem;
        }


        .newsletter {
            display: flex;
            flex-direction: column;
            max-width: 350px;
            margin-right: 1.8rem;


            input {
                width: 100%;
                padding: 0.8rem 1rem;
                border: none;
                background: #f7f7f7;
                border-radius: 6px;
                margin: 0.5rem 0 1rem;
            }


            button {
                width: fit-content;
                background: #d5426a;
                color: #fff;
                padding: 0.6rem 1.2rem;
                border-radius: 6px;
                border: none;
                cursor: pointer;
                font-weight: 600;
            }
        }


    .social {
        margin-top: 3rem;
        display: flex;
        justify-content: center;
        width: 100%;
        gap: 1.2rem;

        img {
            display: flex;
            align-content: center;
            width: 30px;
            height: 30px;
            cursor: pointer;
        }
    }
}

</style>