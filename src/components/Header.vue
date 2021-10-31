<template>
    <header>
        <nav class="menu">
            <ul class="menu-list">
                <li class="menu-list__item">
                    <a class="menu-list-item__link menu-list-item__link--active" href="#">Blog</a>
                    <a class="menu-list-item__link" href="#">Sobre</a>
                    <a class="menu-list-item__link" href="#">Descrição</a>
                </li>
            </ul>
        </nav>
        <section class="header-home">
            <img class="header-home__logo" alt="Toula e Iago" src="../assets/img/toula-e-iago.jpg">
            <div class="header-home__content">
                <h1 class="header-home-content__title">Toula & Iago</h1>
                <p class="header-home-content__description">
                    Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.
                </p>
            </div>
        </section>
    </header>
</template>

<script>
    export default {
        name: 'Header'
    }
</script>

<style scoped>
    header {
        align-items: center;
        background: rgb(47, 85, 141);
        color: #fdfdfd;
        grid-area: cabecalho;
        padding: 1rem 8rem 2rem 8rem;
    }

    .menu {
        display: flex;
        justify-content: center;
    }

    .menu-list {
        list-style: none;
        padding: 0;
    }

    .menu-list-item__link {
        color: #fdfdfd;
        padding: .5rem 1rem;
        text-decoration: none;
    }

    .menu-list-item__link:first-child {
        padding-left: 0;
    }

    .menu-list-item__link:hover, .menu-list-item__link--active {
        font-weight: bold;
    }

    .header-home {
        align-items: center;
        display: flex;
        margin: 20px 10px;
    }

    .header-home__logo {
        border-radius: 50%;
        width: 20%;
        height: 20%;
        min-width: 20%;
        min-height: 20%;
    }

    .header-home__content {
        padding-left: 60px;
    }

    .header-home-content__description {
        font-size: 13px;
        line-height: 1.8;
        text-align: justify;
        font-family: 'Roboto', sans-serif;
        padding-top: 1rem;
    }

    @media screen and (max-width: 425px) {
        header {
            padding: 1rem 1rem 1rem 1rem;
        }

        .header-home-content__description {
            display: none;
        }
    }

    @media screen and (max-width: 768px) {
        .header-home-content__description {
            font-size: 12px;
        }
    }
</style>