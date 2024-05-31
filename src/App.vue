<script >
import AppHeader from './components/AppHeader.vue';
import AppFooter from './components/AppFooter.vue';
import AppLista from './components/AppLista.vue';

export default {
    name: 'MyApp',
    data() {
        return {
            test: 'test'
        }
    },
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
    <!--Main con dentro il tag per future bagine con main differente-->
    <main>
        <AppLista />
    </main>
    <AppFooter />
</template>

<style></style>
