<template>
    <div class="container">
        <div class="row">
            <div class="col-3" v-for="(coktail, index) in coktail_list" :key="index" >
                <CardComponent :coktail="coktail"/>
            </div>
        </div>
    </div>
</template>

<script>
    import axios from 'axios';
import CardComponent from './CardComponent.vue'
    export default {
        name: 'CardList',
        component: {
            CardComponent,
        },
        data() {
            return {
                api_path:'www.thecocktaildb.com/api/json/v1/1/filter.php?a=Alcoholic',
                coktail_list: [],
            }
        },
        mounted() {
            axios.get(this.api_path)
                .then((response) => {
                    this.coktail_list=response.data.drinks
            })
        }
    }
</script>

<style lang="scss" scoped>

</style>