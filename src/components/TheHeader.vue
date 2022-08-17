<template>
    <header>
        <div class="main-container-header">
            <div class="logo-container-header">
                <div class="logo-header">
                    GuiCardilho
                </div>
            </div>

            <div class="links-container-header">
                <a href="#Home" class="links-header">Home</a>
                <a href="#Projetos" class="links-header">Projetos</a>
                <a href="#Estudos" class="links-header">Conhecimentos</a>
                <a href="#Contato" class="links-header">Contato</a>
            </div>
        </div>
    </header>
</template>

<script>
import { defineComponent } from 'vue';
    export default defineComponent({
            name: 'TheHeader',
    })
</script>

<style>
    @import url('https://fonts.googleapis.com/css2?family=Righteous&display=swap');
    @import url('https://fonts.googleapis.com/css2?family=Satisfy&display=swap');

    .main-container-header{
        display: flex;
        align-items: center;
        justify-content: space-between;
        width: 100%;
        height: 70px;
        background-color: #030303;
    }

    .logo-header{
        color: #fff;
        font-family: 'Satisfy', cursive;
        margin-left: 200px;
        font-size: 30px;
    }

    .links-header{
        text-decoration: none;
        color: white;
        transition: 0.5s;
        text-transform: uppercase;
        margin: 0px 20px;
        font-family: 'Righteous', cursive;
    }
    .links-header:last-child{
        margin-right: 100px;
        
    }

    .links-header:hover{
        color: #E0E722;
    }
</style>