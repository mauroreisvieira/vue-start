<template>
    <nav class="navigation" role="navigation" aria-hidden="true">
        <router-link
            class="navigation__item"
                v-for="(menu, index) in this.menus"
                :key="index"
                :to="menu.path"
                :title="menu.name" >
                {{ menu.name }}
        </router-link>
    </nav>
</template>

<script>
    export default {
        data: function () {
            return {
                menus: [
                    { path: '/', name: 'Home' },
                    { path: '/about', name: 'About' }
                ]
            }
        },
        mounted() {}
    }
</script>
