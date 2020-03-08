<template>
    <div class="[ row ]">
        <div v-for="recipe in recipes" :key="recipes" class="[ col-sm-12 ]">
            <recipeComponent        v-bind:thumbnail="recipe.thumbnail"
                                    v-bind:title="recipe.title"
                                    v-bind:ingredients="recipe.ingredients"
                                    v-bind:website="recipe.href"

            ></recipeComponent>
        </div>
    </div>
</template>

<script>
import recipeComponent from './recipeComponents.vue'

export default {
    name: 'recipePage',
    components: {
        recipeComponent
    },
    data(){
        return{
            recipes: []
        }
    },
    mounted() {
    const convensionUrl = 'https://cors-anywhere.herokuapp.com/';
    const url = 'http://www.recipepuppy.com/api';

        fetch(convensionUrl + url)
        .then(function(response) {
            return response.json();
        })
        .then(result => {
            console.log(result)
            this.recipes = result.results;
        })
    }
}
</script>