<template>
    <div class="main-content__item">
        <a class="main-content-item__link" v-bind:class="{'main-content-item__link--active': activeClass }" href="#">
            {{ newsTitle }}
        </a>
        <p class="main-content-item__description">{{ newsDescription }}</p>
    </div>
</template>

<script>
    export default {
        name: 'ContentItem',
        props: {
            activeClass: Boolean,
            newsTitle: String,
            newsDescription: String
        }
    }
</script>

<style scoped>
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
</style>