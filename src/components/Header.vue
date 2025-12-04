<script setup>
import logo from "../assets/logo.png"
// import { Icon } from "@iconify/vue"
import pessoa from "../assets/pessoa.png"
import busca from "../assets/busca.png"
import menu from "../assets/menu.png"

</script>

<template>

<header>
    <img :src="logo" alt="">
    <nav>
      <ul>
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
                <img :src="pessoa" alt="">
            </a>
        </li>
      </ul>  
        
    </nav>
   
</header>

</template>

<style scoped lang="scss">

    header{
        
        display: flex;
        justify-content: space-between;
        align-items: center;
        flex-wrap: wrap;
        margin: 2rem;

        ul{
            display: flex;
            gap: 1.5rem;
            flex-wrap: wrap;
            list-style: none;
        }

        a{
            text-decoration: none;
            color: black;
        }
    }

</style>