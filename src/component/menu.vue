<template>
    <header>
        <a class="logo" href="#"><img src="../asset/svg/logo.svg" alt="logo"></a>
        <!-- bur-->
        <a class="mobile-menu-toggle js-toggle-menu hamburger-menu" :class="{ 'open' : menuOpen }" @click="ctrlMenu($event);">
            <span class="menu-item"></span>
            <span class="menu-item"></span>
            <span class="menu-item"></span>
        </a>
        <!-- M Menu-->
        <nav class="mobile-nav-wrap" role="navigation">
            <ul class="mobile-header-nav" :class="{ 'show' : menuOpen }">
                <li @click="ctrlPos($event, 'worker')"><a class="line" href="" @click.prevent.self><span class="icon"><img src="../asset/svg/star_w.svg" alt=""></span><span>智能人才</span></a></li>
                <li @click="ctrlPos($event, 'learning')"><a class="line" href="" @click.prevent.self><span class="icon"><img src="../asset/svg/book_w.svg" alt=""></span><span>學習發展</span></a></li>
                <li @click="ctrlPos($event, 'welfare')"><a class="line" href="" @click.prevent.self><span class="icon"><img src="../asset/svg/good_w.svg" alt=""></span><span>優質福利</span></a></li>
            </ul>
        </nav>
        <!-- PC menu -->
        <nav class="pc_nav">
            <ul>
                <li @click="ctrlPos($event, 'worker')"><a class="line" href="" @click.prevent.self><img src="../asset/svg/star.svg" alt=""><span>智能人才</span></a></li>
                <li @click="ctrlPos($event, 'learning')"><a class="line" href="" @click.prevent.self><img src="../asset/svg/book.svg" alt=""><span>學習發展</span></a></li>
                <li @click="ctrlPos($event, 'welfare')"><a class="line" href="" @click.prevent.self><img src="../asset/svg/good.svg" alt=""><span>優質福利</span></a></li>
            </ul>
        </nav>
    </header>
</template>

<script>
    export default {
        name: 'menu',
        data () {
            return {
                menuOpen: false
            }
        },
        methods: {
            ctrlMenu: function(evt){
                evt.preventDefault();
                this.menuOpen = !this.menuOpen;
            },
            ctrlPos: function(evt, name){
                evt.preventDefault();
                var pos = document.querySelector('.'+name).offsetTop;
                this.$parent.scrollToY(pos, 500);
                this.menuOpen = false;
            }
        }
    }
</script>

<style>
    .mobile-header-nav{
        overflow: hidden;
        display: block;
        height: 0px;
        -webkit-transition: height .5s ease;
        transition: height .5s ease;
    }
    .mobile-header-nav.show{
        display: block;
        height: 312px;
        -webkit-transition: height .5s ease;
        transition: height .5s ease;
    }
</style>