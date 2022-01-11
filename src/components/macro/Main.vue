<template>
    <main>
        <Jumbo/>
        <Books/>
        <Process/>
        <Message/>
    </main>
</template>

<script>
import Jumbo from '../sections/Jumbo.vue'
import Books from '../sections/Books.vue'
import Process from '../sections/Process.vue'
import Message from '../sections/Message.vue'

export default {
    name: 'Main',
    components: {
        Jumbo,
        Books,
        Process,
        Message
    }
}
</script>

<style lang="scss" scoped>

</style>