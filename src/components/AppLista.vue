<script >
import ListaCard from './ListaCard.vue';
export default {
    name: 'AppLista',
    components: {
        ListaCard,
    },
    data() {
        return {
            "products": [
                {
                    "id": 1,
                    "frontImage": "/public/img/1.webp",
                    "backImage": "/public/img/1b.webp",
                    "brand": "Levi's",
                    "name": "Relaxed Fit",
                    "price": 29.99,
                    "isInFavorites": true,
                    "badges": [
                        {
                            "type": "tag",
                            "value": "Sostenibilità"
                        },
                        {
                            "type": "discount",
                            "value": "-50%"
                        }
                    ]
                },
                {
                    "id": 2,
                    "frontImage": "/public/img/2.webp",
                    "backImage": "/public/img/2b.webp",
                    "brand": "Guess",
                    "name": "Roses Tee",
                    "price": 20.99,
                    "isInFavorites": true,
                    "badges": [
                        {
                            "type": "discount",
                            "value": "-30%"
                        }
                    ]
                },
                {
                    "id": 3,
                    "frontImage": "/public/img/3.webp",
                    "backImage": "/public/img/3b.webp",
                    "brand": "Come Zucchero Filato",
                    "name": "Voglia di colori pastello",
                    "price": 129.99,
                    "isInFavorites": false,
                    "badges": [
                        {
                            "type": "discount",
                            "value": "-30%"
                        }
                    ]
                },
                {
                    "id": 4,
                    "frontImage": "/public/img/4.webp",
                    "backImage": "/public/img/4b.webp",
                    "brand": "Levi's",
                    "name": "Tee Unisex",
                    "price": 14.99,
                    "isInFavorites": false,
                    "badges": [
                        {
                            "type": "tag",
                            "value": "Sostenibilità"
                        },
                        {
                            "type": "discount",
                            "value": "-50%"
                        }
                    ]
                },
                {
                    "id": 5,
                    "frontImage": "/public/img/5.webp",
                    "backImage": "/public/img/5b.webp",
                    "brand": "Maya Deluxe",
                    "name": "Stripe Bodice",
                    "price": 99.99,
                    "isInFavorites": true,
                    "badges": [
                        {
                            "type": "tag",
                            "value": "Sostenibilità"
                        },
                        {
                            "type": "discount",
                            "value": "-50%"
                        }
                    ]
                },
                {
                    "id": 6,
                    "frontImage": "/public/img/6.webp",
                    "backImage": "/public/img/6b.webp",
                    "brand": "Esprit",
                    "name": "Maglione - Black",
                    "price": 29.99,
                    "isInFavorites": true,
                    "badges": [
                        {
                            "type": "tag",
                            "value": "Sostenibilità"
                        }
                    ]
                }
            ]
        };
    },
};
</script>

<template>
    <div class="container">
        <div class="riga">
            <div class="col-33" v-for="(product, index) in products" :key="index">
                <ListaCard :img="product.frontImage" :backImage="product.backImage" :marca="product.brand"
                    :nome="product.name" :prezzo="product.price" />
            </div>
        </div>
    </div>
</template>

<style scoped>
.riga {
    display: flex;
    flex-wrap: wrap;
}

.col-33 {
    width: calc(100% / 3);
}
</style>