<template>
  <div class="">
   <div class="header-app mt-4 mb-4 p-2">
    <CButton style="height: 100%;" color="dark" shape="rounded-pill"> Home </CButton>
    <CButton> Portfolio </CButton>
    <CButton> Transcript </CButton>
   </div>
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
   <div class="core-skills mt-5 mb-5">
      <h3 class="mb-4">Core Skills</h3>
      <div class="skills-container"> 
        <div v-for="skill in coreSkills" class="skill-box m-1 p-4">
          <div class="col-12"><img class="mb-3" :src="skill.img" width="50px" height="50px"></div>
          <div class="col-12"><span>{{ skill.name }}</span></div>
        </div>
      </div>
   </div>
   <div class="core-skills mt-5 mb-5">
      <h3 class="mb-4">Soft Skills</h3>
      <div class="skills-container"> 
        <div v-for="skill in softSkills" class="skill-box m-1 p-4">
          <div class="col-12"><img class="mb-3" :src="skill.img" width="50px" height="50px"></div>
          <div class="col-12"><span>{{ skill.name }}</span></div>
        </div>
      </div>
   </div>
 
  </div>
</template>

<script>
import '@/utils/kangy.css'
import { CButton} from '@coreui/vue'


export default {
  name: 'Dashboard',
  components: {


  },
  data(){
    return {
      coreSkills:[
      {img:'https://upload.wikimedia.org/wikipedia/commons/f/f1/Vue.png',name:'Vue'},
      {img:'https://avatars.githubusercontent.com/u/36859861?s=280&v=4',name:'CoreUI'},
      {img:'https://upload.wikimedia.org/wikipedia/commons/thumb/b/b2/Bootstrap_logo.svg/1200px-Bootstrap_logo.svg.png',name:'Bootstrap5'},
      {img:'https://upload.wikimedia.org/wikipedia/commons/6/6a/JavaScript-logo.png',name:'Javascript'} ,   
      {img:'https://cdn-icons-png.flaticon.com/512/732/732212.png',name:'HTML5'} ,
      {img:'https://upload.wikimedia.org/wikipedia/commons/thumb/6/62/CSS3_logo.svg/800px-CSS3_logo.svg.png',name:'CSS'},
      {img:'https://upload.wikimedia.org/wikipedia/commons/thumb/3/3f/Git_icon.svg/2048px-Git_icon.svg.png',name:'Git'},
      {img:'https://cdn-icons-png.freepik.com/512/6261/6261546.png',name:'Responsive Design'}       
    ],
    softSkills:[
      {img:'https://cdn-icons-png.flaticon.com/512/3065/3065945.png',name:'Communication'},
      {img:'https://cdn-icons-png.freepik.com/512/5985/5985765.png',name:'Creativity'},
      {img:'https://cdn-icons-png.flaticon.com/512/6213/6213303.png',name:'Collaboration'},
      {img:'https://cdn-icons-png.flaticon.com/512/9815/9815843.png',name:'Time Management'} ,   
      {img:'https://cdn-icons-png.flaticon.com/512/6487/6487594.png',name:'Problem Solving'} ,   
    ]
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
.core-skills{
  width: 100%;
  text-align: center;
}
.skills-container{
  width: 100%;
  overflow-x: scroll;
  display: -webkit-inline-box;
}
.skill-box{
  width: 150px;
  aspect-ratio: 1/1;
  background-color:rgb(39, 39, 39);
  border-radius: 25px;
}
</style>
