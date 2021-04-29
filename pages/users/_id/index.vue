<template>
    <h1>A single user, with ID: {{ $route.params.id }}</h1> 
    <!-- if you named the file user it would be $route.params.user -->
</template>

<script>
export default {
    //special method nuxt executes before rendering a route //
    validate (data) {
        console.log(data);
        //page only loadable with parent id of 1 //
        // return data.params.id == 1;

        // regex check for only numbers
        return /^\d+$/.test(data.params.id)
    }
}
</script>
