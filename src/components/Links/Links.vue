<template>
    <div class="links_container">
        <a class="link" href="https://twitter.com/alex_arizola" rel="noopener noreferrer" target="_blank">
            Twitter
        </a>

        <a class="link" href="https://instagram.com/alex.arizola" rel="noopener noreferrer" target="_blank">
            Instagram
        </a>

        <a class="link" href="https://www.threads.net/@alex.arizola" rel="noopener noreferrer" target="_blank">
            Threads
        </a>

        <a class="link" href="https://instagram.com/alex.arizola" rel="noopener noreferrer" target="_blank">
            Portfolio
        </a>

        <a class="link" href="https://www.linkedin.com/in/alexander-arizola/" rel="noopener noreferrer" target="_blank">
            LinkedIn
        </a>

        <a class="link" href="mailto:alexarizola46@gmail.com" rel="noopener noreferrer" target="_blank">
            Email
        </a>
    </div>
</template>

<script lang="ts">
    import { Vue } from 'vue-class-component';

    export default class Links extends Vue {}
</script>

<!-- Add "scoped" attribute to limit SCSS to this component only -->
<style scoped lang="scss">
    .links_container {
        margin-top: 1.5vmin;

        display: flex;
        flex-direction: column;

        > .link {
            &:hover {
                color: rgb(0, 38, 255);
                background: rgba(255, 255, 255);
            }

            width: 70vmin;
            padding: 2vh;

            margin-bottom: 2vmin;
            text-align: center;
            text-decoration: none;

            font-family: Arial, sans-serif;
            font-size: 1.75vh;
            font-weight: 600;

            color: white;
            cursor: pointer;
            transition: .11s ease-in-out;

            border-radius: 10vh;
            border: .2vh solid white;
        }
    }
</style>
