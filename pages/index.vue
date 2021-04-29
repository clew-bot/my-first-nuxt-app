<template>
  <div class="container">
    <Header />
   <nuxt-link to="/users" id="link">Users</nuxt-link>
    </div>
</template>

<script>
// we can just do '~/components/Header.vue' to skip the dot slashes everywhere
import Header from "~/components/Header"

export default {
  components: {
    Header
  }
}
</script>

<style>


</style>
