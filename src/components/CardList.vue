<template>
    <div class="container">
        <div class="row">
            <div class="col-3">
                <CardComponent />
            </div>
        </div>
    </div>
</template>

<script>
    import CardComponent from './CardComponent.vue'
    export default {
        name: 'CardList',
        component: {
            CardComponent,
        }
    }
</script>

<style lang="scss" scoped>

</style>