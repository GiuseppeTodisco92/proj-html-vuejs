<template>
 <section class="d-flex justify-content-center py-5 text-center ">
    <div class="container_custom ">
      <h2>Request A Free Quote </h2>
      <p class="py-2">Lorem ipsum dolor sit amet consectetur adipisicing elit. Rerum explicabo odit perspiciatis distinctio suscipit! Unde quidem aperiam repudiandae vitae suscipit voluptatem incidunt! Veniam magni deleniti rem dolor ut facilis corrupti.</p>
      <a href="#"><custom-button :NameButton="TextButton"/></a>  
    </div>
  </section>
</template>

<script>
import CustomButton from '../Commons/CustomButton.vue'
export default {

    name: "SectionRequestFreeQuote",
      components: { 
        CustomButton
         },
    data(){
      return{
        TextButton: "click here",
      }
    }
}
</script>

<style lang="scss" scoped>
section{
  height: 25rem;
  background-image: url(../../assets/img/avada-movers-request-quote-background.jpg);
  background-size: cover;
   h2{
      color:var(--tertiary-color);
      font-weight: 700;
    }

    p{
      color:var(--seventary-color);
      font-size: .75rem;
    }
}

</style>