<template>
    <div class="[ card ]">
        <div class="[ row ]">
            <div class="[ col-sm-4 ]">
            <div class="[ col-sm-4 ]"><img :src="thumbnail" /></div>
            <div class="[ col-sm-4 ]"></div>
        </div>
            <div class="[ card--information ]"><br />
                            <b>Title: </b>{{title}}<br />
                            <b>Ingredients: </b>{{ingredients}}<br />
                            <b>Website: </b><a :href="website" target="_blank">Click Here</a><br />
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'recipeComponents',
    props: ['thumbnail','title','ingredients','website'],
}
</script>

<style scoped>
html {
    background-color: darkgrey;
}
.card{
    border: solid 1px black;
    border-radius: 4px;
    padding: 0px 20px 30px;
    margin: 30px 700px 0 700px;
    background-color: darkgrey;
    
}

.card img{
    width: ;
    padding-top: 20px;
}


</style>