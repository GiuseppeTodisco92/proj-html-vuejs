<template>
  <main>
    <SectionHero/>
    <SectionAward/>
  </main>
</template>

<script>
import SectionAward from '../Section/SectionAward.vue'
import SectionHero from '../Section/SectionHero.vue'
export default {
 
    name: 'BaseMain',
    components: { 
        SectionHero,
        SectionAward,
        
         }
}
</script>

<style>

</style>