<template>
    <Header></Header>
    <Content></Content>
    <Footer></Footer>
</template>

<script>
    import Header from './components/Header.vue'
    import Content from './components/Content.vue'
    import Footer from './components/Footer.vue'

    export default {
        name: 'App',
        components: {
            Header,
            Content,
            Footer
        }
    }
</script>

<style>
    #app {
        background: #f1f1f1;
        display: grid;
        font-family: Arial, Helvetica, sans-serif;
        grid-template-areas:
            "cabecalho"
            "conteudo"
            "rodape";
        grid-template-columns: auto;
        grid-template-rows: 350px auto auto;
        font-family: 'Roboto Slab', serif;
    }

    @media screen and (max-width: 425px) {
        #app {
            grid-template-rows: 150px auto auto;
        }
    }
</style>