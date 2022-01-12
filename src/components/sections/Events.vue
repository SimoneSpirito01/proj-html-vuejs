<template>
    <section>
        <div class="my_container">
            <div class="my_card">
                <div class="top">
                    <div class="image">
                        <img src="../../assets/img/h-2-blog-img-1.jpg" alt="">
                    </div>
                    <div class="tag">
                        <div class="green">
                            <span>07</span>
                        </div>
                        <div class="pink">
                            <div class="text">may '19</div>
                            <div class="triangles">
                                <span class="left"></span>
                                <span class="right"></span>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="bottom">
                    <div class="title">
                        This way, loves: a detailed guide through new design
                    </div>
                    <div class="by">
                        By Emily Fields
                    </div>
                </div>
            </div>
            <div class="my_card">
                <div class="top">
                    <div class="image">
                        <img src="../../assets/img/h-2-blog-img-2.jpg" alt="">
                    </div>
                    <div class="tag">
                        <div class="green">
                            <span>07</span>
                        </div>
                        <div class="pink">
                            <div class="text">may '19</div>
                            <div class="triangles">
                                <span class="left"></span>
                                <span class="right"></span>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="bottom">
                    <div class="title">
                        I try to give people a different way of looking art
                    </div>
                    <div class="by">
                        By Emily Fields
                    </div>
                </div>
            </div>
            <div class="my_card">
                <div class="top">
                    <div class="image">
                        <img src="../../assets/img/h-2-blog-img-3.jpg" alt="">
                    </div>
                    <div class="tag">
                        <div class="green">
                            <span>07</span>
                        </div>
                        <div class="pink">
                            <div class="text">may '19</div>
                            <div class="triangles">
                                <span class="left"></span>
                                <span class="right"></span>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="bottom">
                    <div class="title">
                        Introduce Richard Laperrière of those amazing features
                    </div>
                    <div class="by">
                        By Emily Fields
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'Events'
}
</script>

<style lang="scss" scoped>

    section {
        padding: 140px 0;

        .my_container {
            display: flex;

            .my_card {
                width: calc(100% / 3 - 24px);
                margin: 0 12px;

                .top {
                    position: relative;

                    .image {
                        overflow: hidden;
                    }

                    img {
                        width: 100%;
                        display: block;
                        transition: transform 0.5s;
                        cursor: pointer;

                        &:hover {
                            transform: scale(1.05);
                        }
                    }

                    .tag {
                        position: absolute;
                        top: -15px;
                        left: 15px;
                        text-align: center;
                        

                        .green {
                            background-color: #c0e1cf;
                            display: flex;
                            justify-content: center;
                            align-items: center;
                            box-shadow: rgba(99, 99, 99, 0.2) 0px 2px 8px 0px;
                            height: 40px;
                            padding-bottom: 8px;
                            
                            span {
                                font-size: 35px;
                                font-style: italic;
                                font-weight: bold;
                                font-family: 'Playfair Display', serif;
                            }

                        }

                        .pink {
                            font-size: 11px;
                            font-weight: bold;
                            text-transform: uppercase;
                            letter-spacing: 2px;
                            

                            .text {
                                background-color: #f3d0c7;
                                padding: 4px 7px;

                            }

                            .triangles {
                                width: 100%;
                                display: flex;
                                justify-content: center;
                                
                                span {
                                    width: 0;
                                    height: 0;
                                    border-style: solid;
                                    border-width: 12px 35px 0 0;
                                    border-color: #f3d0c7 transparent transparent transparent;

                                    &.right {
                                        border-width: 0 35px 12px 0 ;
                                        border-color: transparent #f3d0c7 transparent transparent;

                                    }
                                }
                            }
                        }
                    }
                }

                .bottom {

                    .title {
                        font-size: 23px;
                        margin-top: 27px;
                        margin-bottom: 17px;
                    }

                    .by {
                        font-size: 14px;
                        font-style: italic;
                        font-family: 'Playfair Display', serif;
                    }
                }
            }
        }
    }

</style>