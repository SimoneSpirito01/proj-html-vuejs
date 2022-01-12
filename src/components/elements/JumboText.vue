<template>
    <div class="left">
        <h1>{{title}} <span>{{lastWord}}</span></h1>
        <p>{{text}}</p>
        <div class="my_btn">
            <button>Read more</button>
        </div>
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
        margin-right: 100px;
        display: flex;
        flex-direction: column;
        justify-content: center;
        width: 35%;

        @media (max-width: 1500px) {
            width: 45%;
            margin-right: 20px;;
            padding-right: 70px;
        }

        h1 {
            font-size: 85px;
            font-weight: 300;

            @media (max-width: 1500px) {
                font-size: 65px;
            }

            span {
                font-weight: bold;
                font-style: italic;
                font-family: 'Playfair Display', serif;
            }
        }

        p {
            font-size: 18px;
            font-weight: 200;
            margin: 20px 0 30px;
            padding: 0;
            color: rgb(109, 109, 109);
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