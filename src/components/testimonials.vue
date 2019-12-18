<template>
  <div class="testimonials-container">
    <div class="testimonial-header">
      <h2>Testimonials</h2>
    </div>
    <div class="testimonial-content">
      <div class="testimonial-content--container" v-for="(data, index) in testimonials" :key="index">
        <div class="testimonial-text">
          {{data.text}}
        </div>
        <div class="testimonial-profile">
          <div class="testimonial-profile--icon">
            <img src="../assets/testimonial.png">
          </div>
          <div class="testimonial-profile--name">
            <h4>{{data.name}}</h4>
            <p>{{data.org}}</p>
          </div>
        </div>
        <div class="testimonial-quotes">
          <img src="../assets/quotes.png">
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data(){
    return{
      testimonials:[
        {
          text:"Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s",
          name:"client name",
          org:"Position, ORG"
        },
        {
          text:"Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book.",
          name:"client name",
          org:"Position, ORG"
        },
        {
          text:"Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s",
          name:"client name",
          org:"Position, ORG"
        }
      ]
    }
  }
}
</script>

