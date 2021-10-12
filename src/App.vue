<template>
    <div id="app">
        <Header></Header>
        <b-row>
            <b-col lg="4">
                <SideMenu />
            </b-col>
            <b-col lg="8">
                <Home />
            </b-col>
        </b-row>
        <Footer>test</Footer>
    </div>
</template>

<script>
import Header from "./layout/Header.vue";
import Footer from "./layout/Footer.vue";
import SideMenu from "./layout/SideMenu.vue";
import Home from "./views/Home.vue";

export default {
    name: "App",
    el: "root",
    components: {
        Header,
        Footer,
        SideMenu,
        Home,
    },
    methods: {
        debug() {
            console.log(this.$root);
        },
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
}
</style>
