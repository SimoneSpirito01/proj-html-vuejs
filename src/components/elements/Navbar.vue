<template>
    <nav>
        <ul>
            <li v-for="(list, i) in nav" :key="i">
                {{list.name}}
                <div class="my_bg"></div>
            </li>
            <li>
                <img src="../../assets/svg/svg-1.svg" alt="nav">
            </li>
        </ul>
    </nav>
</template>

<script>
export default {
    name: 'Navbar',
    data() {
        return {
            nav: [
                {
                    name: 'Home'
                },
                {
                    name: 'Pages'
                },
                {
                    name: 'Portfolio'
                },
                {
                    name: 'Blog'
                },
                {
                    name: 'Shop'
                },
                {
                    name: 'Elements'
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>

    nav {
        ul {
            list-style: none;
            display: flex;
            align-items: center;
            margin: 0;

            li {
                height: 16px;
                font-size: 13px;
                font-weight: bold;
                text-transform: uppercase;
                letter-spacing: 3px;
                margin-left: 40px;
                padding-left: 3px;
                position: relative;
                cursor: pointer;

                .my_bg {
                    position: absolute;
                    bottom: 0;
                    left: 0;
                    width: 0;
                    height: 38%;
                    z-index: -1;
                    transition: width 0.2s;
                }

                &:hover {

                    .my_bg {
                        width: 100%;
                    }
                }

                &:first-child {
                    
                    .my_bg {
                        width: 100%;
                        background-color: rgba(241,207,191,1);
                    }
                }

                &:nth-child(2) {
                    
                    .my_bg {
                        background-color: rgba(230, 226, 209, 1);
                    }
                }
                &:nth-child(3):hover {
                    
                    .my_bg {
                        background-color: rgba(216, 240, 227, 1);
                    }
                }
                &:nth-child(4):hover {
                    
                    .my_bg {
                        background-color: rgba(235, 232, 249, 1);
                    }
                }
                &:nth-child(5):hover {
                    
                    .my_bg {
                        background-color: rgba(254, 242, 189, 1);
                    }
                }
                &:nth-child(6):hover {
                    
                    .my_bg {
                        background-color: rgba(255, 217, 180, 1);
                    }
                }
            }
        }
    }

</style>