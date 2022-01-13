<template>
    <header id="header">
        <Logo/>
        <Navbar/>
    </header>
</template>

<script>
import Logo from '../elements/Logo.vue'
import Navbar from '../elements/Navbar.vue'

export default {
    name: 'Header',
    components: {
        Logo,
        Navbar
    }
}
</script>

<style lang="scss" scoped>

    header {
        height: 90px;
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 0 40px;
    }

</style>