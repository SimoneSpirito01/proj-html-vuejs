<template>
    <main>
        <Jumbo/>
        <Books/>
        <Process/>
        <Message/>
        <Events/>
    </main>
</template>

<script>
import Jumbo from '../sections/Jumbo.vue'
import Books from '../sections/Books.vue'
import Process from '../sections/Process.vue'
import Message from '../sections/Message.vue'
import Events from '../sections/Events.vue'

export default {
    name: 'Main',
    components: {
        Jumbo,
        Books,
        Process,
        Message,
        Events
    }
}
</script>

<style lang="scss" scoped>

</style>