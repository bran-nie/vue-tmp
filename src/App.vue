<template>
    <div id="app">
        <img alt="Vue logo" src="./assets/logo.png" />
        <Select v-show="v" />
        <Password />
        <HelloWorld v-show="v" msg="Welcome to Your Vue.js App" />
    </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue';
import Select from './components/Select';
import Password from './components/Password';

export default {
    name: 'App',
    data() {
        return {
            v: false,
        };
    },
    components: {
        HelloWorld,
        Select,
        Password,
    },
};
</script>

<style>
#app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
}
</style>
