<template>
    <TheHome id="Home"></TheHome>
    <TheProjetos id="Projetos"></TheProjetos>
    <TheEstudos id="Estudos"></TheEstudos>
    <TheContato id="Contato"></TheContato>
</template>

<script>
    import { defineComponent } from 'vue';
    import TheHome from './conteudo/TheHome.vue'
    import TheProjetos from './conteudo/TheProjetos.vue'
    import TheEstudos from './conteudo/TheEstudos.vue'
    import TheContato from './conteudo/TheContato.vue'

    export default defineComponent({
        name: 'TheConteudo',
        components:{
            TheHome,
            TheProjetos,
            TheEstudos,
            TheContato,
        },

    });
</script>