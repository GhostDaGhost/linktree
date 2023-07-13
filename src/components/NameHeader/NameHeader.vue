<template>
    <div>
        <div class="nameheader_container">
            <h1 class="nameheader">Alex Arizola</h1>
        </div>

        <div class="role_container">
            <h2 class="role">Full Stack Developer</h2>
        </div>

        <div class="favoritequote_container">
            <h3 class="favoritequote">"I'm just a simple man, trying to make my way in the universe." - Jango Fett</h3>
        </div>
    </div>
</template>

<script lang="ts">
    import { Vue } from 'vue-class-component';

    export default class NameHeader extends Vue {}
</script>

<!-- Add "scoped" attribute to limit SCSS to this component only -->
<style scoped lang="scss">
    @import url('https://fonts.googleapis.com/css2?family=Comfortaa:wght@300;400;500;600;700&display=swap');

    .nameheader_container {
        margin-top: 3vmin;
        text-align: center;

        > .nameheader {
            font-size: 2.35vh;
            font-family: Arial, Helvetica, sans-serif;
            color: white;
        }
    }

    .role_container {
        margin-top: 1vmin;
        text-align: center;

        > .role {
            font-size: 1.7vh;
            font-family: 'Comfortaa';
            color: rgb(206, 206, 206);
        }
    }

    .favoritequote_container {
        margin-top: 3.5vmin;
        text-align: center;

        > .favoritequote {
            font-style: italic;
            font-size: 1.6vh;
            font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;

            color: white;
            user-select: text;
        }
    }
</style>
