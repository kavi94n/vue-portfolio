<template>
  <nav id="home" class="nav">
    <div  class="flex justify-end px-3 py-3 ">
      <button @click="scroll('home')" class="text-lg">Home</button>
      <button @click="scroll('about')" class="text-lg">About</button>
      <button @click="scroll('contact')" class="text-lg">Portfolio </button>
      <button @click="scroll('project')" class="text-lg">Project</button>
      <button @click="scroll('contact')" class="text-lg">Contact</button>
    </div>
  </nav>
</template>

<script>



export default {
  name: 'NavBar',

  methods: {
    scroll(refName) {
      const element = document.getElementById(refName);
      element.scrollIntoView({behavior: "smooth"});
  }
}
}
</script>

<style scoped>
.nav{
  background-color: rgb(19, 241, 207);
}

button{
  border: 2px black solid ;
  border-radius: 5px;
  margin-left: 20px;
  padding: 3px;
  background-color: rgb(19, 139, 115);
}

</style>


