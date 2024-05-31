<script >
import AppHeader from './components/AppHeader.vue';
import AppFooter from './components/AppFooter.vue';
import AppLista from './components/AppLista.vue';

export default {
    name: 'MyApp',
    components: {
        AppHeader,
        AppFooter,
        AppLista
    },
};
</script>

<template>
    <!--scrivo qui la mia struttura HTML-->
    <AppHeader />
    <main>
        <AppLista />
    </main>
    <AppFooter />
</template>

<style></style>
