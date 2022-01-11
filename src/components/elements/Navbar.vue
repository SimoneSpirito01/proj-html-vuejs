<template>
    <nav>
        <ul>
            <li v-for="(list, i) in nav" :key="i">{{list.name}}</li>
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
                cursor: pointer;

                &:not(:last-child):hover, &:first-child {
                    background: rgb(255,255,255);
                    background: linear-gradient(180deg, rgba(255,255,255,1) 60%, rgba(241,207,191,1) 60%);
                }

                &:nth-child(2):hover {
                    background: linear-gradient(180deg, rgba(255,255,255,1) 60%, rgba(230, 226, 209, 1) 60%);
                }

                &:nth-child(3):hover {
                    background: linear-gradient(180deg, rgba(255,255,255,1) 60%, rgba(216, 240, 227, 1) 60%);
                }

                &:nth-child(4):hover {
                    background: linear-gradient(180deg, rgba(255,255,255,1) 60%, rgba(235, 232, 249, 1) 60%);
                }

                &:nth-child(5):hover {
                    background: linear-gradient(180deg, rgba(255,255,255,1) 60%, rgba(254, 242, 189, 1) 60%);
                }

                &:nth-child(6):hover {
                    background: linear-gradient(180deg, rgba(255,255,255,1) 60%, rgba(255, 217, 180, 1) 60%);
                }
            }
        }
    }

</style>