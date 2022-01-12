<template>

    <div class="right">
        <div class="image girl">
            <img src="../../assets/img/h-2-slider-img-15.png" alt="" class="my_background">
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
            <img src="../../assets/img/h-2-slider-img-16.png" alt="" class="my_background">
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

</template>

<script>
export default {
    name: 'Jumboimg3'
}
</script>

<style lang="scss" scoped>

    .right {
        display: flex;
        margin-top: 70px;

        > * {
            position: relative;
            // width: 100%;

            // .my_background {
            //     width: 80%;
            // }

            .my_background {
                width: 380px;

                @media (max-width: 1500px) {
                    width: 253px;
                }
            }

        }
            
        .girl {
            transform: translateX(25px);
        }   
        
        .green {
            position: absolute;
            bottom: 0;
            left: -30px;
        }

        .multi {
            position: absolute;
            bottom: 0;
            right: -90px;
        }

        .pink-l {
            position: absolute;
            top: -40px;
            left: 10px;
        }

        .pink-r {
            position: absolute;
            top: 50px;
            right: 0;
        }

        .violet {
            position: absolute;
            top: -60px;
            right: 50px;
        }

        .brown {
            position: absolute;
            bottom: 180px;
            left: -70px;
        }

    }

</style>