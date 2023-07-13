<template>
    <div class="favicon_container">
        <img class="favicon" alt="favicon" src="../../assets/logo.png" draggable="false">
    </div>
</template>

<script lang="ts">
    import { Vue } from 'vue-class-component';

    export default class Favicon extends Vue {}
</script>

<!-- Add "scoped" attribute to limit SCSS to this component only -->
<style scoped lang="scss">
    @keyframes rotateEffect {
        from {
            transform: rotateY(0deg);
        }
        to {
            transform: rotateY(360deg);
        }
    }

    .favicon_container {
        margin-top: 20px;

        > .favicon {
            width: 96px;
            height: 96px;

            animation-name: rotateEffect;
            animation-duration: 2500ms;
            animation-iteration-count: infinite;
            animation-timing-function: linear; 
        }
    }
</style>
