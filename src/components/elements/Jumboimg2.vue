<template>
    <div class="right">
        <div class="image couple">
            <img src="../../assets/img/h-2-slider-img-11.png" alt="">
            <div class="image green">
                <img src="../../assets/img/h-2-slider-img-13.png" alt="">
            </div>
            <div class="image pink-l">
                <img src="../../assets/img/short-slider-rev-1-img-2.png" alt="">
            </div>
            <div class="image brown">
                <img src="../../assets/img/h-2-slider-img-12.png" alt="">
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
    name: 'Jumboimg2'
}
</script>

<style lang="scss" scoped>

    .right {
        display: flex;

        > * {
            position: relative;
            
            > img {
                width: 800px;
            }
        }

        .image {

            .image {
                position: absolute;
            }
        }

        .couple {
            position: relative;

            .green {
                bottom: 0;
                left: 15px;
            }

            .brown {
                bottom: 80px;
                left: -70px;
            }

            .pink-l {
                top: 120px;
                left: -15px;
            }

            .pink-r{
                top: 0px;
                right: 80px;
            }

            .violet {
                bottom: 17px;
                right: 50px;
            }
        }
    }    

</style>