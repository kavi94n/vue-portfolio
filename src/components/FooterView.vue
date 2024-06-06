<template >
  <footer id="contact" class="foot">
    <div class="max-w-4xl mx-auto">
      <div class="flex flex-wrap">
        <div class="col-md-6 w-full md:w-1/2">
          <h3 class="text-xl font-semibold mb-4">Leave a Comment</h3>
          <form>
            <div class="form-group">
              <label for="name"></label>
              <input type="text" class="form-control" id="name" placeholder="Enter your name">
            </div>
            <div class="form-group mt-5">
              <label for="email"></label>
              <input type="email" class="form-control" id="email" placeholder="Enter your email">
            </div>
            <div class="form-group mt-5">
              <label for="message"></label>
              <textarea class="form-control" id="message" rows="3"></textarea>
            </div>
            <button type="submit" class="border 1px border-black mt-3 bg-green-800 mb-10 rounded-md p-2">Submit</button>
          </form>
        </div>
        <div class="col-md-6">
          <h3 class="text-xl font-semibold mb-4">Contact Me</h3>
          <ul class=" list-none">
            <li class="mb-2">
              <a class="text-white-600 hover:text-blue-600  " href="https://github.com/your-username" target="_blank">
                <font-awesome-icon   icon="fa-brands fa-github" /> <br> Github
              </a>
            </li>
            <li class="mb-2">
              <a class="text-black-600 hover:text-blue-800" href="https://twitter.com/your-username" target="_blank">
                <font-awesome-icon icon="fa-brands fa-twitter" /> <br> Twiter
              </a>
            </li>
            <li class="mb-2">
              <a class="text-black-600 hover:text-blue-800" href="https://www. linkedin.com/in/your-username/" target="_blank">
                <font-awesome-icon icon="fa-brands fa-linkedin" /> <br> Linkedin
              </a>
            </li>

          </ul>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome'
import {  library } from '@fortawesome/fontawesome-svg-core'
import { faGithub, faTwitter,faLinkedin } from '@fortawesome/free-brands-svg-icons'

 library.add(faGithub, faTwitter, faLinkedin )

export default {
  name: 'Footer',
  components: {
    FontAwesomeIcon,
  },
}
</script>

<style scoped>
.foot{
   background-color: rgb(19, 139, 115);
   color: white;
   padding: 4px;
}



</style>

