<template>
    <main>
        <Jumbo/>
        <Books/>
    </main>
</template>

<script>
import Jumbo from '../sections/Jumbo.vue'
import Books from '../sections/Books.vue'

export default {
    name: 'Main',
    components: {
        Jumbo,
        Books
    }
}
</script>

<style lang="scss" scoped>

</style>