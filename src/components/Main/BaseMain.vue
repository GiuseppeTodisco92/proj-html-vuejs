<template>
  <main>
    <SectionHero/>
    <SectionAward/>
    <SectionFullService/>
    <SectionFreeQuote/>
    <SectionTestimonials/>
    <SectionRequestFreeQuote/>
  </main>
</template>

<script>
import SectionAward from '../Section/SectionAward.vue'
import SectionFreeQuote from '../Section/SectionFreeQuote.vue'
import SectionFullService from '../Section/SectionFullService.vue'
import SectionHero from '../Section/SectionHero.vue'
import SectionRequestFreeQuote from '../Section/SectionRequestFreeQuote.vue'
import SectionTestimonials from '../Section/SectionTestimonials.vue'
export default {
 
    name: 'BaseMain',
    components: { 
        SectionHero,
        SectionAward,
        SectionFullService,
        SectionFreeQuote,
        SectionTestimonials,
        SectionRequestFreeQuote,
        
         }
}
</script>

<style>

</style>