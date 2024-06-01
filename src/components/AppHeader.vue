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
    <header>
        <div class="container d-flex flex-command">
            <HeaderList />
            <HeaderLogo />
            <HeaderIcone />
        </div>
    </header>
</template>

<style></style>