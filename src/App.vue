<template>
  <nav>
  
  <router-view></router-view>
  <projects :projects="projects" />
  <FooterView/>
  </nav>
  
</template>

<script>

import FooterView from './components/FooterView.vue'
import projects from './components/Project.vue'


export default {
  name: 'App',
  components:{
    projects,
    FooterView,
    
  },
  data() {
    return {
      projects: [
        { id: 1,
           name: "Crée le CV avec HTMLet CSS  ",
           date: "01/12/2023",
           imageUrl: require('./assets/18.png'),
           hover: false,
           
        },
        { id: 2,
           name: "Crée une space commentaire ",
           date:"07/02/2024",
           imageUrl: require('./assets/19.jpg'),
           hover: false,

        },
        { id: 3,
          name: "Crée le chaier de charge",
          date:"01/04/2024",
          imageUrl: require('./assets/20.jpg'),
          hover: false,

        },
      ]
    }
  }
  

  

  }

</script>

<style scoped>
name{
  color: blue;
}
</style>