<template>
  <section class="d-flex justify-content-center align-items-center">
    <div class="container text-center">
      <h4>we are a professional</h4>
      <h2>Full-service Solution</h2>
    
      <div class="row container justify-content-center">
          <CardService class="col-2" v-for="(card,index) in cards" :key="index"  :card="card" />
      </div>

    </div>
  </section>
</template>

<script>
import CardService from '../Commons/CardService.vue'
export default {
  components: { CardService },
    name: "SectionFullService",
    data(){
      return{
        cards:[
      {
        image:'avada-movers-serviceonephoto-final-200x128.jpg',
        title:"Two Man Teams",
        text:"lorem ipsum dolor sit arnet,consectetur adipiscing elit. Nullam ac consectetur augue. Orci varius naotque penatibus et magnis dis parturient montes,nascetur ridiculus mus."
      },
      {
        image:'avada-movers-servicetwophoto-final-200x128.jpg',
        title:"We Do All The Lifting",
        text:"lorem ipsum dolor sit arnet,consectetur adipiscing elit. Nullam ac consectetur augue. Orci varius naotque penatibus et magnis dis parturient montes,nascetur ridiculus mus."
      },
      {
        image:'avada-movers-servicethreephoto-final-200x128.jpg',
        title:"Coast to Coast",
        text:"lorem ipsum dolor sit arnet,consectetur adipiscing elit. Nullam ac consectetur augue. Orci varius naotque penatibus et magnis dis parturient montes,nascetur ridiculus mus."
      },
    ]
      }
    }
}
</script>

<style lang="scss" scoped>
section{
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