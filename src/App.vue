<template>
    <div id="app">
        <nav class="navbar is-dark">
            <div class="navbar-brand">
                <a class="navbar-item" href="#">
                    MyComplany
                </a>
                <div class="navbar-burger burger" v-on:click="toggleNav" v-bind:class="{ 'is-active': isActive }"
                     data-target="navbarExampleTransparentExample">
                    <span></span>
                    <span></span>
                    <span></span>
                </div>
            </div>
            <div id="navbarExampleTransparentExample" class="navbar-menu" v-bind:class="{ 'is-active': isActive }">
                <div class="navbar-end">
                    <router-link to="/" class="navbar-item">Home</router-link>
                    <router-link to="faq" class="navbar-item">About</router-link>
                    <router-link to="faq" class="navbar-item">FAQ</router-link>
                    <div class="navbar-item">
                        <div class="field is-grouped">
                            <p class="control">
                                <a class="button is-primary" href="#">
                                  <span class="icon">
                                    <i class="fas fa-download"></i>
                                  </span>
                                    <span>Join Now</span>
                                </a>
                            </p>
                        </div>
                    </div>
                </div>
            </div>
        </nav>

        <router-view></router-view>

        <footer class="footer is-primary">
            <div class="container">
                <div class="columns">
                    <div class="column">
                        <p>
                            Footer
                        </p>
                    </div>
                    <div class="column has-text-right">
                        <a class="icon" href="#"><i class="fab fa-facebook-f"></i></a>
                        <a class="icon" href="#"><i class="fab fa-twitter"></i></a>
                    </div>
                </div>
            </div>
        </footer>
    </div>
</template>
<script>
    export default {
        name: 'app',
        data: function () {
            return {
                isActive: false
            }
        },
        methods: {
            toggleNav: function () {
                this.isActive = !this.isActive;
            }
        }
    }
</script>

<style lang="sass">
    @import '../node_modules/bulma/bulma.sass'
    @import 'mq'

    footer
        background-color: $primary !important
        color: #fff

        .icon
            color: #fff
            margin-left: 20px
</style>