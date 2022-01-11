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

            li {
                font-size: 10px;
                font-weight: bold;
                text-transform: uppercase;
                letter-spacing: 3px;
                margin-left: 40px;
                padding-left: 3px;
                cursor: pointer;

                &:not(:last-child):hover, &:first-child {
                    background: rgb(255,255,255);
                    background: linear-gradient(180deg, rgba(255,255,255,1) 60%, rgba(241,207,191,1) 65%);
                }
            }
        }
    }

</style>