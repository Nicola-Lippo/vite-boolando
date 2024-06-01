<script >
import FooterText from './FooterText.vue';
import FooterIcone from './FooterIcone.vue';
export default {
    name: 'AppFooter',
    components: {
        FooterText,
        FooterIcone
    }
}
</script>

<template>
    <footer>
        <div class="container d-flex flex-command">
            <FooterText />
            <FooterIcone />
        </div>
    </footer>
</template>

<style></style>