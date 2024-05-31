<script >
import HeaderList from './HeaderList.vue';
import HeaderLogo from './HeaderLogo.vue';
import HeaderIcone from './HeaderIcone.vue';
export default {
    name: 'AppHeader',
    components: {
        HeaderList,
        HeaderLogo,
        HeaderIcone
    }
}

</script>

<template>
    <div>header</div>
    <HeaderList />
    <HeaderLogo />
    <HeaderIcone />
</template>

<style></style>