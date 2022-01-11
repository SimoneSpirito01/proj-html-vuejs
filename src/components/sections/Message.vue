<template>
    <section>
        <h2>Want to work with us? Send us <span>a message!</span></h2>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Blanditiis nemo incidunt, labore ea officiis similique molestias voluptas at delectus amet fuga aperiam quam expedita quisquam? Sapiente perspiciatis assumenda et commodi fuga vel aut!</p>
        <button>Contact</button>
    </section>
</template>

<script>
export default {
    name: 'Message'
}
</script>

<style lang="scss" scoped>

    section {
        background-image: url('../../assets/img/h-2-background-1.jpg');
        background-size: cover;
        background-position: center;
        padding: 150px 320px 100px;
        text-align: center;

        h2 {
            font-size: 60px;
            margin-bottom: 40px;

            span {
                font-weight: bold;
                font-style: italic;
                font-family: 'Playfair Display', serif;
            }
        }

        p {
            font-size: 18px;
            color: #6d6d6d;
            margin-bottom: 40px;
        }

        button {
            font-size: 13px;
            font-weight: bold;
            text-transform: uppercase;
            letter-spacing: 3px;
            background-color: #d8f0e3;
            padding: 17px 60px;
            border: none;
        }
    }

</style>