<template>
    <div class="right">
        <div class="image bench">
            <img src="../../assets/img/short-slider-rev-1-img-3.png" alt="" class="my_background">
            <div class="image green">
                <img src="../../assets/img/short-slider-rev-1-img-1.png" alt="">
            </div>
            <div class="image green-lite">
                <img src="../../assets/img/short-slider-rev-1-img-8.png" alt="">
            </div>
            <div class="image green-big">
                <img src="../../assets/img/short-slider-rev-1-img-9.png" alt="">
            </div>
            <div class="image pink-l">
                <img src="../../assets/img/short-slider-rev-1-img-2.png" alt="">
            </div>
            <div class="image brown">
                <img src="../../assets/img/short-slider-rev-1-img-10.png" alt="">
            </div>
            <div class="image cloud-brown">
                <img src="../../assets/img/short-slider-rev-1-img-4.png" alt="">
            </div>
            <div class="image cloud-green">
                <img src="../../assets/img/short-slider-rev-1-img-5.png" alt="">
            </div>
            <div class="image pink-r">
                <img src="../../assets/img/short-slider-rev-1-img-6.png" alt="">
            </div>
            <div class="image violet">
                <img src="../../assets/img/short-slider-rev-1-img-7.png" alt="">
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Jumboimg'
}
</script>

<style lang="scss" scoped>

    .right {
        display: flex;

        > * {
            position: relative;
            // width: 100%;

            // > img {
            //     width: 90%;
            // }

            .my_background {
                width: 500px;

                @media (max-width: 1500px) {
                    width: 400px;
                }
            }
            
        }

        .image {

            .image {
                position: absolute;

                @media (max-width: 1500px) {
                    transform: scale(0.8);
                }


                
            }
        }

        .bench {
            position: relative;

            .green {
                bottom: 35px;
                left: -130px;
            }

            .green-lite {
                bottom: 40px;
                right: -20px;
            }

            .green-big {
                bottom: 35px;
                right: -130px;

                @media (max-width: 1500px) {
                    bottom: 25px;
                }
            }

            .brown {
                bottom: 35px;
                right: -190px;
            }

            .pink-l {
                left: -90px;
                bottom: 260px;

                @media (max-width: 1500px) {
                    bottom: 220px;
                }
            }

            .pink-r {
                right: -80px;
                bottom: 260px;

                @media (max-width: 1500px) {
                    bottom: 220px;
                }
            }

            .violet {
                bottom: 40px;
                left: 10px;
            }

            .cloud-brown {
                top: 40px;
                right: -120px;
                z-index: 10;

            }

            .cloud-green {
                top: 31px;
                right: -180px;
            }
        }
    }

</style>