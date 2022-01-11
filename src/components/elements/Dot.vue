<template>
    <div class="circle">
        <div class="top" :class="circle.type" v-html="circle.icon"></div>
        <div class="bottom">
            <div class="title">{{circle.title}}</div>
            <div class="text">{{circle.text}}</div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Dot',
    props: {
        circle: Object
    }
}
</script>

<style lang="scss" scoped>

    .circle {
        text-align: center;

        .top {

            font-size: 47px;
            width: 160px;
            aspect-ratio: 1;
            border-radius: 50%;
            background-color: #faf7f1;
            display: flex;
            justify-content: center;
            align-items: center;
            margin: 0 auto;

            &.bulb {
                color: #badac9;
            }
            &.comment {
                color: #f8d12d;
            }
            &.cloud {
                color: #80465f;
            }
            &.pencil {
                color: #eb6950;
            }
        }

        .bottom {
            margin-top: 22px;
            padding: 0 15px;

            .title {
                font-size: 20px;
                margin-bottom: 13px;
            }

            .text {
                font-weight: 200;
                color: rgb(109, 109, 109);
            }
        }
    }

</style>