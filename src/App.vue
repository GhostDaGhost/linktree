<template>
    <div class='main_container'>
        <div class='columns'>
            <Favicon/>
            <NameHeader/>
            <Links/>

            <div class='madewith_container'>
                <h4 class='madewith'>
                    Created with <a class="hyperlink" href="https://vuejs.org/" rel="noopener noreferrer" target="_blank">Vue.js</a>
                </h4>
            </div>
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
        //min-height: 100vh;

        background-repeat: no-repeat;
        // background: radial-gradient(circle, rgb(58, 159, 206) 20%, rgb(57, 54, 233) 100%);
        background-image: url('./assets/background.jpg');
    }

    ::-webkit-scrollbar {
        display: none;
    }

    .hyperlink {
        &:hover {
            color: rgb(61, 253, 253);
        }

        color: rgb(24, 180, 180);
        transition: .1s ease-in-out;
    }

    .main_container {
        display: flex;
        justify-content: center;

        > .columns {
            display: flex;
            align-items: center;
            flex-direction: column;

            > .madewith_container {
                margin-top: 1vmin;
                text-align: center;

                > .madewith {
                    font-size: 1.85vh;
                    font-family: Arial, sans-serif;
                    color: white;
                }
            }
        }
    }
</style>
