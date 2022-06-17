<template>
  <div class="card_testimonial">
    <img :src="require('@/assets/img/' + card.image)" :alt="card.title">
    <h3>{{card.title}}</h3>
    <p>{{card.text}}</p>

  </div>
</template>

<script>
export default {
    name: "CardTestimonial",
    props:{
        card:Object,
    }
}
</script>

<style lang="scss" scoped>
.card_testimonial{
 padding: 30px 0px;
  margin: 2.5rem;

  img{
  border-radius: 100%;
  width: 100px;
}
h3{
    padding: 1.25rem 0rem;
    color: var(--secondary-color);
    font-size: 1rem;
    font-weight: bold;
  }

p{
    font-size: .625rem;
    font-style: italic;
  }

}


</style>