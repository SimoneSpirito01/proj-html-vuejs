<template>
    <div class="tags">
        <div class="first">
            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 87 87" style="height:40px" fill="#ee2852"><path d="M55.4 81.5c6.1-11.1 5.2-16.1-4.3-24.3 6.1-3.5 9.5-8.5 9.1-15.7-.5-8.2-7.7-14.7-16.3-14.6-8.5.1-15.6 6.7-15.9 15-.3 8.5 5.9 15.8 14.3 16.6 1.4.1 2.8.2 4.2.5 5.9 1.2 10.2 6.7 9.8 12.6-.4 6.4-5.5 11.4-11.8 11.7-19.6.9-38.6-14.8-41.3-34C-.1 26.9 14.4 6.8 36.4 2.8c22.3-4 43.4 10 48.1 32 4.3 20-8.6 41.2-28.4 46.7h-.7z"/></svg>
        </div>
        <div class="second">
            <img src="../../assets/svg/svg-6.svg" alt="">
        </div>
    </div>
</template>

<script>
export default {
    name:'SideTags'
}
</script>

<style lang="scss" scoped>

    .tags {
        position: fixed;
        right: 0;
        top: 200px;

        .first, .second {
            width: 44px;
            aspect-ratio: 1;
            box-shadow: rgba(99, 99, 99, 0.2) 0px 2px 8px 0px;
            display: flex;
            justify-content: center;
            align-items: center;
            cursor: pointer;
            z-index: 100;

        }

        .first {
            background-color: #ef2853;

            svg {
                width: 30px;

                path {
                    fill: white;
                }
            }

            
        }

        .second {
            background-color: white;
            margin-top: 10px;

            img {
                width: 17px;
                margin-right: 1px;
            }
        }
    }

</style>