<template>
    <div class="app">
        <Nav />
        <router-view />
    </div>
</template>

<script>
    import Nav from './scripts/components/Nav.vue'

    export default {
        name: 'app',
        components: { Nav },
        data: function () {
            return {}
        },
        mounted() {
        }
    }
</script>

<style lang="scss">
  @import "./styles/app.scss";
</style>
