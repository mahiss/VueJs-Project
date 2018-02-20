<template>
    <div class="home">
        <section class="hero is-medium is-danger is-bold">
            <div class="hero-body">
                <div class="container">
                    <h1 class="title">
                        {{ heading }}
                    </h1>
                    <div class="is-two-thirds column is-paddingless">
                        <h2 class="subtitle is-4">
                            {{ subheading }}
                        </h2>
                    </div>
                    <a class="button is-large is-warning" id="learn">
                        Learn More
                    </a>
                </div>
            </div>
        </section>
        <section class="section">
            <div class="container" id="learn">
                <div class="columns pd is-desktop">
                    <div class="column is-1 has-text-centered">
                        <i class="fas fa-cog is-primary"></i>
                    </div>
                    <div class="column is-one-third-desktop">
                        <p class="title">
                            <strong>Lorem Ipsum is simply dummy text of the printing and typesetting industry.</strong>
                        </p>
                    </div>
                    <div class="column">
                        <p> Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an
                            unknown printer took a galley of type and scrambled it to make a type specimen book. It has
                            survived not only five centuries, but also the leap into electronic typesetting, remaining
                            essentially unchanged.</p>
                    </div>
                </div>
            </div>
            <div class="columns pd">
                <div class="column">
                    <div class="card">
                        <div class="card-content">
                            <p class="title">
                                “There are two hard things in computer science: cache invalidation, naming things, and
                                off-by-one errors.”
                            </p>
                            <p class="subtitle"> Jeff Atwood </p>
                        </div>
                    </div>
                </div>
                <div class="column">
                    <div class="card">
                        <div class="card-content">
                            <p class="title">
                                “There are two hard things in computer science: cache invalidation, naming things, and
                                off-by-one errors.”
                            </p>
                            <p class="subtitle"> Jeff Atwood </p>
                        </div>
                    </div>
                </div>
                <div class="column">
                    <div class="card">
                        <div class="card-content">
                            <p class="title">
                                “There are two hard things in computer science: cache invalidation, naming things, and
                                off-by-one errors.”
                            </p>
                            <p class="subtitle"> Jeff Atwood </p>
                        </div>
                    </div>
                </div>
            </div>
        </section>
    </div>
</template>

<!--suppress JSAnnotator -->
<script>
    export default {
        name: 'home',
        data(){
            return{
                heading:'Font Awesome Pro',
                subheading:'Level up your Awesome with more icons, styles, & tools!'
            }
        }
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="sass" scoped>
    @import '../mq'

    .hero
        .title
            +mobile
                font-weight:bold
            +tablet
                font-size: 2.5rem
            +desktop
                font-size: 4rem
                margin-top: 2rem
    h2
        margin: 1.5rem 0 2rem 0 !important

    .fa-cog
        font-size: 40px

    #learn
        margin-bottom: 2rem

    .card
        .title
            font-weight: normal
            font-size: 1.6rem;

</style>
