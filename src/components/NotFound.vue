<template>
  <div>
    <h1>404 - Page Not Found</h1>
    <button @click="goBack">go back</button>
  </div>
</template>


<script>
export default {
  name:"NotFound",
  methods:{
    goBack(){
      return this.$router.go(-1)
    },

  },
};
</script>