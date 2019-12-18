<template>
  <div class="banner-container" :style="{ background: 'radial-gradient(ellipse at center, rgba(51,51,51,0.78) 99%, rgba(51,51,51,0.78) 100%), url(' + backgroundImage + ')' }">
     <div class="banner-content">
       <div class="banner-heading">
         <h2>Integer bibendium sit amet arcu vel egestas</h2>
        </div>
       <div class="banner-services">
         <div class="service-content" v-for="(data,index) in services" :key="index">
           <div class="service-content--icon">
             <img :src=data.img />
           </div>
           <p>{{data.name}}</p>
         </div>
       </div>
     </div>
  </div>
</template>
<script>
export default {
  data(){
    return{
      backgroundImage: require('../assets/banner.png'),
      services:[
        {
          name:'Service Name',
          img:require('../assets/people.png')
        },
        {
          name:'Service Name',
          img:require('../assets/service.png')
        },
        {
          name:'Service Name',
          img:require('../assets/setting.png')
        },
      ]
    }
  }
}
</script>

