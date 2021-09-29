<template>
    <main>
        <div class="general-content-formatting">
            <section class="content">
                <h2>-->Content goes here </h2>
            </section>

            <section class="site-features">

            </section>
        </div>

    </main>
</template>

<script>
export default {
    name:'Main'
}
</script>

<style lang="scss" scoped>
@import '../style/variables.scss';

    main{
        h2{
            color: white;
            padding: 1.25rem 0;
        }
        .site-features{
            background-color: $site-features_primary_background_color;
        }
    }
</style>