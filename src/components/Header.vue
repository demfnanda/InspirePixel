<script setup>
import logo from "../assets/logo.png"
// import { Icon } from "@iconify/vue"
import pessoa from "../assets/pessoa.png"
import busca from "../assets/busca.png"

</script>

<template>

<header>
    <img :src="logo" alt="">
    <nav>
        <li>
            <a href="">
               <img :src="busca" alt=""> <!-- NÃO ESQUECER DE COLOCAR OS : ANTES DO SRC-->
            </a>
        </li>
        <li>
            <a href="">Início</a>
        </li>
        <li>
            <a href="">Galeria</a>
        </li>
        <li>
            <a href="">Favoritos</a>
        </li>
        <li>
            <a href="">
                <img src="" alt="">
            </a>
        </li>
    </nav>
   
</header>

</template>

<style scoped lang="scss">
    header{
        border: solid;
        display: flex;
        justify-content: space-between;
        align-items: center;
        flex-wrap: wrap;
        margin: 2rem;
    }
</style>