<template>
    <footer>
        <div class="my_container">
            <div class="my_col">
                <Logo/>
                <div class="text">Let's Get Creative</div>
            </div>
            <div class="my_col">
                <div class="text">
                    <span>
                        {{info.email}}
                        <div class="my_bg"></div>
                    </span>
                    
                </div>
                <div class="text">
                    <span>
                        {{info.cell}}
                        <div class="my_bg"></div>
                    </span>
                </div>
            </div>
            <div class="my_col">
                <div class="text">
                    <span>
                        {{info.address}}
                        <div class="my_bg"></div>
                    </span>
                </div>
                <div class="text">
                    <span>
                        {{info.city}}
                        <div class="my_bg"></div>
                    </span>
                </div>
            </div>
            <div class="my_col">
                <div class="text">Stay in touch with us</div>
                <div class="text d-flex justify-content-between">
                    <i class="fab fa-twitter"></i>
                    <i class="fab fa-pinterest-p"></i>
                    <i class="fab fa-facebook-f"></i>
                    <i class="fab fa-linkedin-in"></i>
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
import Logo from '../../components/elements/Logo.vue'

export default {
    name: 'Footer',
    components: {
        Logo
    },
    data() {
        return {
            info: {
                email: 'maree.qode@gmail.com',
                cell: '+44645 321 789',
                address: "Avenue d'Auderghem 10",
                city: '1040 Brussels, Belgium'
            }
        }
    }
}
</script>

<style lang="scss" scoped>

    footer {
        background-color: #c0e1cf;
        padding: 80px 0;

        .my_container {
            display: flex;
            align-items: center;

            .my_col {
                margin-right: 12%;

                @media (max-width: 1500px) {
                    margin-right: 10%;
                }

                &:first-child {

                    .text:last-child {
                        margin: 0 0 18px;
                    }
                }

                &:nth-child(2), &:nth-child(3) {

                    .text {
                        
                        span {
                            position: relative;
                            z-index: 10;
                        }

                        .my_bg {
                            position: absolute;
                            bottom: 0;
                            left: 0;
                            width: 0;
                            height: 40%;
                            z-index: -1;
                            transition: width 0.4s;
                            background-color: #e1c0b0;
                        }

                        &:hover {

                            .my_bg {
                                width: 100%;
                            }

                        }
                    }
                }

                .text {
                    font-weight: 200;
                    font-size: 15px;
                    color: black;
                    cursor: pointer;

                    &:last-child {
                        margin-top: 10px;
                    }

                    svg {
                        transition: transform 0.5s;

                        &:hover {
                            transform: scale(1.2);
                        }
                    }
                }
            }
        }
    }

</style>