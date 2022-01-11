<template>
    <div class="content w-100" @mouseover="card.hover = true" @mouseleave="card.hover = false">
        <img :src="card.url" alt="">
        <div class="tag" :class="{ visible: card.hover}">
            <div class="title">{{card.title}}</div>
            <div class="text">Illustration</div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Card',
    props: {
        card: Object
    }
}
</script>

<style lang="scss" scoped>

    img {
        display: block;
        width: 100%;
    }

    .tag {
        position: absolute;
        top: 50%;
        background-color: white;
        padding: 20px;
        transform: translate(-10px, -50%);
        transition: opacity 200ms ease-in-out, transform 200ms ease-in-out;
        opacity: 0;

        &.visible {
            opacity: 1;
            transform: translate(0, -50%)
        }
        

        .title {
            font-size: 26px;
            margin-bottom: 8px;
        }

        .text {
            font-style: italic;
            font-family: 'Playfair Display', serif;
        }
    }

</style>