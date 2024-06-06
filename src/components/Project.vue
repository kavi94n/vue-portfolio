<template>
  <h1>Mes Projets</h1>
  <div  id="project" class="project">
   
        <tr class="box" v-for="project in projects" :key="project.id"  @mouseover="project.hover = true"
      @mouseleave="project.hover = false">
      <div >
          <h2 class="name">{{ project.name }}</h2>
          <p class="date">{{ project.date }}</p>
          <div class="image-container">
        <img :src="project.imageUrl" :alt="project.name" class="project-image" />
        <button v-if="project.hover" class="open-button">Open</button>
      </div>
      </div>
    </tr>
  </div>
</template>

<script>
export default {
  name:'projects',
  props:{
    projects:Array
  }
  
}
</script>


<style scoped>
.project{
  background-color: rgb(19, 139, 115);
  display: flex;
  justify-content: center;
  border: black solid 1px;

}

.box{
  display: grid;
  justify-content: center;
  justify-items: center;
  border: black solid 1px;
  padding: 5px;
  margin-left:70px;
  height: 350px;
  width: 250px;
  background-color: aquamarine;
  cursor: pointer;

}

h1{
  display: flex;
  justify-content: center;
  font-family:serif;
  font-size: 30px;
  background-color: rgb(19, 139, 115);
}

img{
  height: 290px;
}



.project-image:hover {
  transform: scale(1.2);
}

.open-button {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%) scale(0.8);
  padding: 10px 20px;
  background-color: rgba(0, 0, 0, 0.7);
  color: white;
  border: none;
  border-radius: 5px;
  cursor: pointer;
  transition: opacity 0.3s ease, transform 0.3s ease;
  opacity: 0;
  visibility: hidden;
}

.open-button {
  opacity: 0;
}

.image-container:hover .open-button {
  opacity: 1;
  transform: translate(-50%, -50%) scale(1.2);
}
</style>

