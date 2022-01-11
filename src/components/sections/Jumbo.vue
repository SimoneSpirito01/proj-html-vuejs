<template>
    <!-- <div class="jumbo">
        <div class="skip">
            <div>
                <i class="fas fa-chevron-left"></i>
            </div>
        </div>
        <div class="content">
            <div class="left">
                <h1>Devotion that never <span>ends</span></h1>
                <p>Neque portto quisquam est, qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit, sed quia non numquam euis modi.</p>
            </div>
            <div class="right">
                <div class="image girl">
                    <img src="../../assets/img/h-2-slider-img-15.png" alt="">
                    <div class="image green">
                        <img src="../../assets/img/h-2-slider-img-13.png" alt="">
                    </div>
                    <div class="image pink-l">
                        <img src="../../assets/img/short-slider-rev-1-img-2.png" alt="">
                    </div>
                    <div class="image brown">
                        <img src="../../assets/img/h-2-slider-img-12.png" alt="">
                    </div>
                </div>
                <div class="image man">
                    <img src="../../assets/img/h-2-slider-img-16.png" alt="">
                    <div class="image multi">
                        <img src="../../assets/img/h-2-slider-img-17.png" alt="">
                    </div>
                    <div class="image pink-r">
                        <img src="../../assets/img/short-slider-rev-1-img-6.png" alt="">
                    </div>
                    <div class="image violet">
                        <img src="../../assets/img/h-2-slider-img-14.png" alt="">
                    </div>
                </div>
            </div>
        </div>
        <div class="skip">
            <div>
                <i class="fas fa-chevron-right"></i>
            </div>
        </div>
    </div> -->
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
        <button class="carousel-control-prev justify-content-start my_control ms-4" type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide="prev">
            <div class="skip">
                <div>
                    <i class="fas fa-chevron-left left"></i>
                </div>
            </div>
        </button>
        <button class="carousel-control-next justify-content-end my_control me-4" type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide="next">
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
        align-items: center;

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

        .my_inner {
            overflow: initial;
            max-height: 430px;
        }

        .my_control {
            width: 10%;
            opacity: 1;
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

            


        }
    }

</style>