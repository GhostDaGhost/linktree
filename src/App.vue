<template>
    <div class='main_container'>
        <div class='columns'>
            <Favicon/>
            <NameHeader/>
            <Links/>
        </div>
    </div>
</template>

<script lang="ts">
    import { Options, Vue } from 'vue-class-component';

    import Favicon from './components/Favicon/Favicon.vue';
    import Links from './components/Links/Links.vue';
    import NameHeader from './components/NameHeader/NameHeader.vue';

    @Options({components: {
        Favicon,
        NameHeader,
        Links
    }})

    export default class App extends Vue {}
</script>

<style lang="scss">
    * {
        user-select: none;
    }

    body {
        min-height: 100vh;

        background-repeat: no-repeat;
        // background: radial-gradient(circle, rgb(58, 159, 206) 20%, rgb(57, 54, 233) 100%);
        background-image: url('./assets/background.jpg');
    }

    ::-webkit-scrollbar {
        display: none;
    }

    .main_container {
        display: flex;
        justify-content: center;

        > .columns {
            display: flex;
            align-items: center;
            flex-direction: column;
        }
    }
</style>
