<template>
  <section class="d-flex justify-content-center py-5 text-center ">
    <div class="container_custom ">
      <h4>headache free</h4>
      <h2>Award Winning<br>Moving Company</h2>
      <p class="py-2">Lorem ipsum dolor sit amet consectetur adipisicing elit. Rerum explicabo odit perspiciatis distinctio suscipit! Unde quidem aperiam repudiandae vitae suscipit voluptatem incidunt! Veniam magni deleniti rem dolor ut facilis corrupti.</p>
      <a href="#"><custom-button :NameButton="TextButton"/></a>
    </div>
  </section>
</template>

<script>
import CustomButton from '../Commons/CustomButton.vue'
export default {
  
    name: "SectionAward",
    components: { 
      CustomButton
       },
    data(){
      return{
        TextButton: "read our testimonials",
      }
    }
}
</script>

<style lang="scss" scoped>
section{
  background-color: var(--eightary-color);
  height: 31.25rem;
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

    p{
      color:var(--seventary-color);
      font-size: .75rem;
    }
  
  
}


</style>