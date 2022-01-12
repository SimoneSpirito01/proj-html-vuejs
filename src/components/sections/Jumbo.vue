<template>
    <div id="carouselExampleIndicators" class="carousel slide jumbo" data-bs-ride="carousel">
        <div class="carousel-indicators my_indicators">
            <div class="my_button">
                <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="0" class="active" aria-current="true" aria-label="Slide 1"></button>
            </div>
            <div class="my_button">
                <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="1" aria-current="true" aria-label="Slide 2"></button>
            </div>
            <div class="my_button">
                <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="2" aria-current="true" aria-label="Slide 3"></button>
            </div>
        </div>
        <div class="carousel-inner my_inner">
            <div class="carousel-item active">
                <div class="content">
                    <JumboText title="Projects made with" lastWord="love" text="Neque porro quisquam est, qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit, sed quia non numquam euis modi."/>
                    <Jumboimg/>
                </div>
            </div>
            <div class="carousel-item">
                <div class="content">
                    <JumboText title="Our new folio full of" lastWord="joy" text="Neque porro quisquam est, qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit, sed quia non numquam euis modi."/>
                    <Jumboimg2/>
                </div>
            </div>
            <div class="carousel-item">
                <div class="content">
                    <JumboText title="Devotion that never" lastWord="ends" text="Neque porro quisquam est, qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit, sed quia non numquam euis modi."/>
                    <Jumboimg3/>
                </div>
            </div>
        </div>
        <button class="carousel-control-prev justify-content-start my_control ms-5" type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide="prev">
            <div class="skip">
                <div>
                    <i class="fas fa-chevron-left left"></i>
                </div>
            </div>
        </button>
        <button class="carousel-control-next justify-content-end my_control me-5" type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide="next">
            <div class="skip">
                <div>
                    <i class="fas fa-chevron-right right"></i>
                </div>
            </div>
        </button>
    </div>
</template>

<script>
import JumboText from '../elements/JumboText.vue'
import Jumboimg from '../elements/Jumboimg.vue'
import Jumboimg2 from '../elements/Jumboimg2.vue'
import Jumboimg3 from '../elements/Jumboimg3.vue'
import 'bootstrap';



export default {
    name: 'Jumbo',
    components: {
        JumboText,
        Jumboimg,
        Jumboimg2,
        Jumboimg3,
    }
}
</script>

<style lang="scss" scoped>

    .jumbo {
        height: 600px;
        display: flex;
        justify-content: space-between;
        margin-top: 30px;
        overflow-x: hidden;

        @media (max-width: 1500px) {
            margin-top: 70px;
            height: 450px;
        }

        .my_indicators {
            margin-bottom: 0;

            .my_button {
                display: flex;
                align-items: center;

                button {
                    width: 8px;
                    height: 8px;
                    border-radius: 50%;
                    margin: 0 10px;
                    background-color: #e1c0b0;
                    opacity: 1;

                    &.active {
                        width: 11px;
                        height: 11px;
                    }
                }
            }
        }

        .my_inner {
            overflow: initial;
            margin: 0 auto;
            width: 90%;
        }

        .my_control {
            width: initial;
            opacity: 1;
            justify-content: center;

        }

        .skip {

            div {
                width: 32px;
                height: 32px;
                border-radius: 50%;
                color: white;
                background-color: #e1c0b0;
                display: flex;
                justify-content: center;
                align-items: center;

                .left {
                    margin-right: 2px;
                }

                .right {
                    margin-left: 2px;
                }
            }
        }

        .content {
            display: flex;
            justify-content: center;
            align-items: center;

            @media (max-width: 1500px) {
                align-items: flex-end;
            }

        }
    }

</style>