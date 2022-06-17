<template>
  <section>
    <div class="box_free_quote container_custom d-flex justify-content-end align-items-center ">
      <div class="free_quote text-center">
        <h4>we remove the headache from moving</h4>
        <h2>Move With Ease</h2>
        <hr>
        <p>With our super simple service we can take you from getting a quote, right through to begin in your new home with all of you belonginings securely packed and safely delivered, even in the rooms of your choice.</p>
        <custom-button :NameButton="TextButton"/>
      </div>
    </div>

  </section>
</template>

<script>
import CustomButton from '../Commons/CustomButton.vue'
export default {
 
    name: "SectionFreeQuote",
    components: { CustomButton },
    data(){
      return{
        TextButton: "get a free quote now",
      }
    }
}
</script>

<style lang="scss" scoped>
section{
  height: 37.5rem;
  background-image: url(../../assets/img/avada-movers-movewithease-background-new.jpg);
  background-size: cover;
  .box_free_quote{
    width: 100%;
    height: 100%;
    .free_quote{
        color: var(--primary-color);
        width: 25rem;
        padding: 1.25rem;
        margin-right: 1.5625rem;
        background-color: var(--tertiary-color);
        border: .625rem solid var(--quartarary-color);
        h4{
           font-size: .75rem;
           font-weight: bold;
          text-transform: uppercase;
        }

    h2{  
      font-weight: 700;
    }
    p{
      font-size: .625rem;
      padding: .625rem 0rem;
    }
    }
  }
}
</style>