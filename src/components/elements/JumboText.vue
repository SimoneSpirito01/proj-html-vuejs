<template>
    <div class="left">
        <h1>{{title}} <span>{{lastWord}}</span></h1>
        <p>{{text}}</p>
        <button>Read more</button>
    </div>
</template>

<script>
export default {
    name: 'JumboText',
    props: {
        title: String,
        lastWord: String,
        text: String
    }
}
</script>

<style lang="scss" scoped>

    .left {
        width: 30%;
        margin-right: 100px;

        h1 {
            font-size: 75px;
            font-weight: 400;

            span {
                font-weight: bold;
                font-style: italic;
                font-family: 'Playfair Display', serif;
            }
        }

        p {
            margin: 20px 0 30px;
            padding: 0;
            color: #a6a6a6;
        }

        button {
            font-size: 13px;
            font-weight: bold;
            text-transform: uppercase;
            letter-spacing: 3px;
            background-color: white;
            padding: 17px 35px;
            border: 3px solid #e1c0b0;
        }
    }

</style>