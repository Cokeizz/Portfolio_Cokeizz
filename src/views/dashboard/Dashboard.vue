<template>
  <div class="">
   <div class="header-app mt-4 mb-4"></div>
   <div class="mt-4 mb-4" style="display: flex;justify-content: end;"><CBadge style="opacity: 0.9;font-size: small;background-color: greenyellow;color: black;" class="pl-2 pr-2" shape="rounded-pill">OPEN TO WORK</CBadge>&nbsp;</div>
   <div class="about-me">
    <div class="row p-3">
      <div class="col-md-3 col-sm-12 p-4">
              <img class="img-fluid" style="border-radius: 50%;width: 100%;" src="/src/assets/images/me.jpg">
      </div>
      <div class="col-md-9 col-sm-12 p-4">
            <h1>Hi! I'm Coke</h1>
            <div style="color: aliceblue;"> A Computer Science grad from Khon Kaen University, currently a front-end developer at Silom Technology. Passionate about indie game development, UX/UI and digital art </div>
            <hr/>
            <CButton class="contact m-1"><i class="fi fi-sr-envelope"></i></CButton>
            <CButton class="contact m-1"><i class="fi fi-brands-linkedin"></i></CButton>
            <CButton class="contact m-1"><i class="fi fi-brands-line"></i></CButton>
            <CButton class="contact m-1"><i class="fi fi-brands-github"></i></CButton>
      </div>

    </div>
       
   </div>
 
  </div>
</template>

<script>
import '@/utils/kangy.css'
import { CButton, useColorModes, CModal } from '@coreui/vue'

export default {
  name: 'Dashboard',
  components: {

  },
  data(){
    return {
   
  }
  },
  created(){

  },
  computed:{    
  },
  methods:{
  }
}
</script>
<style>
.header-app{
  width: 100%;
  height: 60px;
  background-color: rgb(52, 52, 52);
  opacity: 0.9;
  border-radius: 30px;
}
.about-me{
  width: 100%;
  background-color:rgb(39, 39, 39);
  border-radius: 25px;
}
.bedge{
  background-color: rgb(208, 255, 208);
  color: rgb(46, 139, 57);
}
.contact{
  background-color:rgb(52, 52, 52);
  font-size:x-large;
}
</style>
