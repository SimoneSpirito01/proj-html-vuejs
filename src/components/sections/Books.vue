<template>
    <section>
        <div v-for="(card, i) in cards" :key="i" class="my_card">
            <Card :card="card"/>
        </div>
        
    </section>
</template>

<script>
import Card from '../elements/Card.vue'

export default {
    name: 'Books',
    components: {
        Card
    },
    data() {
        return {
            cards: [
                {
                    url: require('../../assets/img/h-2-port-img-1.jpg'),
                    title: 'All these illustrations',
                    hover: false
                },
                {
                    url: require('../../assets/img/h-2-port-img-2.jpg'),
                    title: 'Type and illustrations',
                    hover: false
                },
                {
                    url: require('../../assets/img/h-2-port-img-3.jpg'),
                    title: 'Draw and illustrate',
                    hover: false
                },
                {
                    url: require('../../assets/img/h-2-port-img-4.jpg'),
                    title: 'Illustrations of novels',
                    hover: false
                },
                {
                    url: require('../../assets/img/h-2-port-img-5.jpg'),
                    title: 'Too many illustrations',
                    hover: false
                },
                {
                    url: require('../../assets/img/h-2-port-img-6.jpg'),
                    title: 'Dream are illustrations',
                    hover: false
                },
            ]
        }
    },
}
</script>

<style lang="scss" scoped>

    section {
        display: flex;
        flex-wrap: wrap;
        margin-top: 20px;

        .my_card {
            width: calc(100% / 3);
            position: relative;
            cursor: pointer;
            overflow: hidden;

            
        }
    }

</style>