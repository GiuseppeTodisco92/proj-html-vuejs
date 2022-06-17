<template>
  <div class="card_service d-flex flex-column ">
    <img :src="require('@/assets/img/' + card.image)" :alt="card.title">
    <div class="text_box">
        <h3>{{card.title}}</h3>
        <p>{{card.text}}</p>
        <custom-button :NameButton="TextButton" />
    </div>
  </div>
</template>

<script>

import CustomButton from './CustomButton.vue'
export default {
    name:"CardService",
    components: { 
        CustomButton
         },
          
    data(){
        return{
            TextButton: "read more",
          
        }
    },

     props:{
                card: Object,
                
            },
}
</script>

<style lang="scss" scoped>
.card_service{
    background-color:var(--quintary-color);
    padding: .625rem;
    margin: 2.5rem;
   

    h3{
        color: var(--secondary-color);
        font-size: 1rem;
        font-weight: bold;
    }

    p{
        font-size: .5rem;
    }

    .text_box{
        background-color: var(--primary-color);
        margin: .625rem 0px;
        padding: 1.875rem .625rem;

       
    }
}
</style>