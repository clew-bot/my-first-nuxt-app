// // template file for index.js and users folder

<template>
  <div>
  <!-- will stay on screen no matter what on /users page because of nested route -->
  <input type="text" v-model="userId">
  <button @click="onLoadUser()">Load User</button>

   <!-- the nuxt child is a replacement for the child component, based on the route
   put what you need that differs in the child -->
  <nuxt-child />
  </div>
</template>

<script>
export default {
  data() {
    return {
      userId: ''
    }
  },
  methods: {
    onLoadUser() {
      this.$router.push('/users/' + this.userId);

    }
  },
  layout: 'users'
}


</script>

<style>

</style>