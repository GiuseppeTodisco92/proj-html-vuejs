<template>
  <section class="d-flex justify-content-center align-items-center">
    <div class="container text-center">
      <h4>happy customers</h4>
      <h2>Testimonals</h2>

      <div class="row justify-content-center">
        <CardTestimonial class="col-4" v-for="(card,index) in cards" :key="index"  :card="card"/>
      </div>
      <custom-button :NameButton="TextButton"/>
    </div>
  </section>
</template>

<script>
import CardTestimonial from '../Commons/CardTestimonial.vue'
import CustomButton from '../Commons/CustomButton.vue'

export default {
 
    name:"SectionTestimonials",
     components: {
      CardTestimonial,
      CustomButton 
      },
    data(){
      return{
        TextButton: "read more testimonials",
        cards:[
      {
        image:'avada-movers-johndoe-final-200x200.jpg',
        title:"jhon Doe",
        text:"lorem ipsum dolor sit arnet,consectetur adipiscing elit. Nullam ac consectetur augue. Orci varius naotque penatibus et magnis dis parturient montes,nascetur ridiculus mus."
      },
      {
        image:'avada-movers-janedoe-final-200x200.jpg',
        title:"Jane Doe",
        text:"lorem ipsum dolor sit arnet,consectetur adipiscing elit. Nullam ac consectetur augue. Orci varius naotque penatibus et magnis dis parturient montes,nascetur ridiculus mus."
      },
      {
        image:'avada-movers-johnsmith-final-200x200.jpg',
        title:"John Smith",
        text:"lorem ipsum dolor sit arnet,consectetur adipiscing elit. Nullam ac consectetur augue. Orci varius naotque penatibus et magnis dis parturient montes,nascetur ridiculus mus."
      },
    ]
      }
    }
}
</script>

<style lang="scss" scoped>
section{
  background-image: url(../../assets/img/avada-movers-testimonial-background.jpg);
  background-size: cover;
  height: 37.5rem;
  h4{
      font-size: .75rem;
      font-weight: bold;
      text-transform: uppercase;
      color: var(--sixtary-color);

    }

    h2{
      color:var(--tertiary-color);
      font-weight: 700;
    }
}
</style>