<script >
export default {
    name: 'ListaCard',
    props: ['img', 'backImage', 'marca', 'nome', 'prezzo']

}
</script>

<template>
    <div class="contenuto">
        <div class="img-shop">
            <img class="img-shop main-img" :src="img" :alt="foto">
            <img class="img-shop hover-img" :src="backImage" :alt="foto">
            <div class="labels">
                <div class="label red">-50 %</div>
                <div class="label green">Sostenibilità</div>
            </div>
            <div class="cuore">
                &hearts;
            </div>
        </div>
        <div>
            <span class="marchio">{{ marca }}</span>
            <p><strong>{{ nome }}</strong></p>
            <span class="prezzo"><strong>{{ prezzo }}</strong></span>
        </div>
    </div>
</template>

<style></style>