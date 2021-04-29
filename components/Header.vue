<template>
  <header class="header">
      <ul class="nav-items">
          <li>
              <nuxt-link to="/users">Users</nuxt-link>
             
          </li>
          <li><nuxt-link to="/home">Home</nuxt-link></li>
          </ul>
  </header>
</template>

<script>
export default {

}
</script>

<style scoped>
.header{
    width: 100%;
    height: 60px;
    display: flex;
   justify-content:center;
    align-items: center;
    background-color: aqua;
}

.nav-items {
   list-style: none;
   padding: 0px;
   margin: 0px;
   display: flex;
    justify-content: space-around;
   align-items: center;
   width: 80%
}

.nav-items a {
    text-decoration: none;
    color: black;
}

</style>