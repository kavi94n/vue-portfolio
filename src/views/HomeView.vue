<template>
  <NavBar/>
   <container id="about">
    <div class="bg">
    <div class="flef">
        <h1 class="font-bold text-5xl py-5 px-10">Hello</h1>
        <h1 class="font-bold text-4xl px-20">I'M Sivalingam Kavirajh</h1>
        <span class="font-semibold text-2xl px-20">Dévolopeur Web</span><br>
        <button >Contact me</button><br>
        <div>
        <img src="17.png" alt="">
      </div>
    </div>
  </div>
    <div class="bg"> 
      <div class="egg"><img  class="pic" src="16.png" alt=""></div>
      <div class="text">
        <h4 class="font-bold" id="About">Je suis un dévelopeur web créative</h4>
          <p>
            Lorem ipsum dolor sit, amet consectetur adipisicing elit.
            Aspernatur, ullam perspiciatis fugiat temporibus laboriosam
            accusamus tempora repellendus sequi sed cum dolorum vero est.
            Placeat dicta architecto reiciendis est veniam. Unde.
          </p><br>
          <p >
            Lorem ipsum dolor sit, amet consectetur adipisicing elit.
            Aspernatur, ullam perspiciatis fugiat temporibus laboriosam
            accusamus tempora repellendus sequi sed cum dolorum vero est.
            Placeat dicta architecto reiciendis est veniam. Unde.
          </p>
      </div>
    </div>
   </container>
</template>


<script>

import Project from '@/components/Project.vue'
import NavBar from '../components/NavBar.vue'
import AboutView from './AboutView.vue'


export default {
  name: 'HomeView',
  components:{
    NavBar,
    AboutView,
    Project,
  }
}
</script>

<style scoped>
.flef{
  background-color: aquamarine;
  font-family: serif;
  border-radius: 10% 30% 0% 50% / 0% 50% 60% 80%;
  height: 400PX;
}



button{
  border: 2px black solid ;
  background-color: #138b73;
  border-radius: 5px;
  padding: 5px;
  width: 200PX;
  margin-left: 20%;
 


}

img{
  height:300px ;
  margin-left: 70%;
  margin-top: -10%;
}

.egg{
  display: block;
  margin-top: 50px;
  height: 300px;
  background-color: #138b73;
  border-radius: 50% 50% 50% 50% / 60% 60% 40% 0%;
  width: 700PX;
  }
  .pic{
    height: 300px;
    margin-left: 15%;
    margin-bottom: 1px;
  }
  .bg{
    background-color: rgb(19, 241, 207);
  }
  .text{
   margin-left: 50%;
   margin-top: -15%;
   padding-bottom: 100px;
   
  }

</style>