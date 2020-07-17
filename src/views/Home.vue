<template>
  <div class="home">
    <Slider />
    <Welcome />
   
    
  </div>
</template>

<script>
// @ is an alias to /src
import Slider from '../components/Slider.vue';
import Welcome from '../components/Welcome.vue';

export default{
  data(){
    return{
      items:[
        {
          src:"https://cdn.pixabay.com/photo/2020/07/11/06/27/diversity-5392891_960_720.png"
        },
        {
          src:"https://cdn.pixabay.com/photo/2020/07/11/06/27/diversity-5392891_960_720.png"
        },
        {
          src:"https://cdn.vuetifyjs.com/images/backgrounds/vbanner.jpg"
        },
      ]
      
    }
  },
  components:{
    Slider,
    Welcome
  }
}

</script>
