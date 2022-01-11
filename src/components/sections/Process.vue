<template>
    <section>
        <h2>Working <span>process</span></h2>
        <div class="process">
            <div v-for="(circle, i) in circles" :key="i">
                <Dot :circle="circle"/>
            </div>
            <div class="my_bg"></div>
        </div>
    </section>
</template>

<script>
import Dot from '../elements/Dot.vue'

export default {
    name: 'Process',
    components: {
        Dot
    },
    data() {
        return {
            circles: [
                {
                    icon: '<i class="fas fa-lightbulb"></i>',
                    title:'First theres an idea',
                    text: 'Lorem ipsum dolor sit, conetu adipisc sed be et ore aliqua pleasure itself',
                    type: 'bulb'
                },
                {
                    icon: '<i class="far fa-comment"></i>',
                    title:'Then we talk about',
                    text: 'Lorem ipsum dolor sit, conetu adipisc sed be et ore aliqua pleasure itself',
                    type: 'comment'
                },
                {
                    icon: '<i class="fas fa-cloud"></i>',
                    title:'And we think about',
                    text: 'Lorem ipsum dolor sit, conetu adipisc sed be et ore aliqua pleasure itself',
                    type: 'cloud'
                },
                {
                    icon: '<i class="fas fa-pencil-alt"></i>',
                    title:'So we draw along',
                    text: 'Lorem ipsum dolor sit, conetu adipisc sed be et ore aliqua pleasure itself',
                    type: 'pencil'
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>

    section {
        padding: 120px 140px;

        h2 {
            font-size: 60px;
            text-align: center;
            margin-bottom: 80px;
            font-weight: 300;

            span {
                font-weight: bold;
                font-style: italic;
                font-family: 'Playfair Display', serif;
            }
        }

        .process {
            
            display: flex;
            justify-content: center;
            position: relative;

            > * {
                width: calc(100% / 4);
            }

            .my_bg {
                width: 80%;
                height: 50%;
                position: absolute;
                background-image: url('../../assets/svg/svg-3.svg');
                background-size: cover;
                background-position: center;
                z-index: -1;
            }
        }
    }

</style>