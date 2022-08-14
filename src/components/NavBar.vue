<template>
    <div class="main-container">
        <div class="center-container">
            <div class="link-container">
                <a href="#Home" class="link-navbar" @click="navBarShow = true">
                    <img class="img-navbar" src="../../public/Imagem/Home.png" />
                    <span class="text-navbar">Home</span>
                </a>
                <a href="#Projetos" class="link-navbar">
                    <img class="img-navbar" src="../../public/Imagem/Portifolio.png" />
                    <span class="text-navbar">Projetos</span>
                </a>
                <a href="#Estudos" class="link-navbar">
                    <img class="img-navbar" src="../../public/Imagem/Educacao.png" />
                    <span class="text-navbar">Conhecimentos</span>
                </a>
                <a href="#Contato" class="link-navbar">
                    <img class="img-navbar" src="../../public/Imagem/Contato.png" />
                    <span class="text-navbar">Contato</span>
                </a>

            </div>
        </div>

    </div>
</template>

<script>
    import { defineComponent } from 'vue';

    export default defineComponent({
        name: 'NavBar',
        data(){
            return{
                navBarShow: false,
            }
        },
    });
</script>

<style scoped>
    @import url('https://fonts.googleapis.com/css2?family=Shadows+Into+Light&display=swap');
    .main-container{
        position: fixed;
        display: flex;
        align-content: center;
        justify-content: center;
        width: 100%;
        top: 92%;
        z-index: 10;
    }

    .center-container{
        background-color: #030303;
        border-radius: 20px;
        padding: 5px 5px;
    }

    .link-container{
        display: flex;
        position: relative;
    }

    .link-navbar{
        margin: 10px 50px;
        text-decoration: none;
        cursor: pointer;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        position: relative;
        transition: 0.5s;
    }


    .img-navbar{
        width: 20px;
        height: 20px;
        transition: 0.5s;
        z-index: 10;
    }

    .link-navbar:hover .img-navbar{
        transform: translateY(-35px);
    }

    .link-navbar::after{
        content: '';
        width: 20px;
        height: 20px;
        padding: 10px;
        border-radius: 15px;
        background-color: #E0E722;
        opacity: 0;
        transition: 0.5s;
        position: absolute;
        box-shadow: 0 0 5px 1px #030303;
        
    }

    .link-navbar:hover::after {
        opacity: 1;
        transform: translateY(-35px);
    }

    .text-navbar{
        position: absolute;
        color: #FFF;
        font-weight: 400;
        font-size: 0.75em;
        letter-spacing: 0.05em;
        transition: 0.5s;
        opacity: 0;
        transform: translateY(20px);
        z-index: 10;
        text-transform: uppercase;
        font-family: 'Shadows Into Light', cursive;
    }

    
    .link-navbar:hover .text-navbar{
        color: #E0E722;
    }

    .link-navbar:hover .text-navbar{
        opacity: 1;
        transform: translateY(10px);
    }


    
    </style>