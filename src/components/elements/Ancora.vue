<template>
    <a href="#header" class="ancora" :class="{visible: visible}">
        <svg version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px" width="20px" height="23px" viewBox="0 0 20 23" enable-background="new 0 0 20 23" xml:space="preserve">
            <line fill="#FFFFFF" stroke="#FFFFFF" stroke-width="2" stroke-linecap="round" stroke-miterlimit="10" x1="10" y1="21.5" x2="10" y2="2.5"></line>
            <g>
                <path fill="#FFFFFF" d="M3.926,7.484c-0.388-0.404-0.388-0.801,0-1.188l5.493-5.493c0.14-0.176,0.334-0.264,0.58-0.264
                s0.44,0.088,0.582,0.264l5.493,5.493c0.387,0.388,0.387,0.784,0,1.188c-0.389,0.405-0.775,0.396-1.162-0.026L9.999,2.599
                L5.088,7.458C4.7,7.88,4.313,7.89,3.926,7.484z"></path>
            </g>
        </svg>
    </a>
</template>

<script>
export default {
    name: 'Ancora',
    data() {
        return {
            visible: false
        }
    },
    methods: {
        myScroll() {
            let x = window.scrollY;
            const booksSection = document.querySelector('.books');
            if (x > booksSection.offsetTop) {
                this.visible = true;
            } else {
                this.visible = false;
            }
        }
    },
    created() {
        window.addEventListener('scroll', this.myScroll)
    }
}
</script>

<style lang="scss" scoped>

    .ancora {
        width: 44px;
        height: 44px;
        background-color: #c0e1cf;
        position: fixed;
        bottom: 22px;
        right: 18px;
        display: flex;
        justify-content: center;
        align-items: center;
        box-shadow: rgba(99, 99, 99, 0.2) 0px 2px 8px 0px;
        opacity: 0;
        transition: opacity 0.4s;

        &.visible {
            opacity: 1;
        }
    }

</style>