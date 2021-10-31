<template>
    <main>
        <h2>Últimas do blog</h2>

        <section class="main-content">
            <ContentItem activeClass newsTitle="Notícia 1" newsDescription="Conteúdo da notícia 1"></ContentItem>
            <ContentItem newsTitle="Notícia 2" newsDescription="Conteúdo da notícia 2"></ContentItem>
            <ContentItem newsTitle="Notícia 3" newsDescription="Conteúdo da notícia 3"></ContentItem>
            <a class="main-content__more-items" href="#">Ver tudo</a>
        </section>
    </main>
</template>

<script>
    import ContentItem from './ContentItem'

    export default {
        name: 'Content',
        components: {
            ContentItem
        }
    }
</script>

<style scoped>
    main {
        grid-area: conteudo;
        margin: 2rem 2rem;
    }

    h2 {
        display: flex;
        justify-content: center;
    }

    .main-content {
        display: grid;
        justify-content: center;
        margin: 2rem;
    }

    .main-content__item {
        margin: 1rem 0rem;
    }

    .main-content-item__link {
        color: rgb(72, 82, 85);
        text-decoration: none;
    }

    .main-content-item__link:hover, .main-content-item__link--active {
        color: rgb(47, 85, 141);
        font-weight: bold;
    }

    .main-content-item__description {
        font-size: 13px;
        color: #333333;
        font-family: 'Roboto', sans-serif;
    }

    .main-content__more-items {
        color: rgb(47,85,141);
        font-weight: bold;
        font-size: 13px;
        text-decoration: none;
    }
</style>