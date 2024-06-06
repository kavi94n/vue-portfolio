<template>
  <div class="not-found">
    <h1>404</h1>
    <p>Page Not Found</p>
    <router-link to="/">Go to Home</router-link>
  </div>
</template>

<script>
export default {
  name: 'NotFound'
}
</script>

<style scoped>
.not-found {
  text-align: center;
  margin-top: 50px;
}

.not-found h1 {
  font-size: 6em;
  margin-bottom: 20px;
}

.not-found p {
  font-size: 1.5em;
  margin-bottom: 20px;
}

.not-found a {
  text-decoration: none;
  color: #42b983;
  font-size: 1.2em;
}
</style>
