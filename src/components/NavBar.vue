<template>
    <div class="main-container">
        <div class="center-container">
            <div class="link-container">   
                <a href="#Home" class="link-navbar"><img class="img-navbar" src="../../public/Imagem/Home.png" /></a>
                <a href="#Projetos" class="link-navbar"><img class="img-navbar" src="../../public/Imagem/Portifolio.png" /></a>
                <a href="#Estudos" class="link-navbar"><img class="img-navbar" src="../../public/Imagem/Educacao.png" /></a>
                <a href="#Contato" class="link-navbar"><img class="img-navbar" src="../../public/Imagem/Contato.png" /></a>
            </div>
        </div>

    </div>
</template>

<script>
    import { defineComponent } from 'vue';

    export default defineComponent({
        name: 'NavBar',
    });
</script>

<style scoped>
    .main-container{
        position: fixed;
        display: flex;
        align-content: center;
        justify-content: center;
        width: 100%;
        top: 90%;
    }

    .center-container{
        background-color: #030303;
        border-radius: 40px;
        padding: 10px 30px;
    }

    .link-navbar{
        margin: 15px;
        text-decoration: none;
        cursor: pointer;
    }

    .img-navbar{
        width: 36px;
        height: 36px;
    }


</style>