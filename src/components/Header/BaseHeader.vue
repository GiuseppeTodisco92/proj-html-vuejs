<template>
  <header class="header">
    <div class="d-flex container justify-content-between align-items-center py-2">
        
        <div class="call" ><i class="fa-solid fa-phone-flip px-2 "></i> Call us for a Free Quote: 1.8000.555.6789</div>
        
        <div class="social">
            <i class="fa-brands fa-facebook-f px-2"></i>
            <i class="fa-brands fa-twitter px-2"></i>
            <i class="fa-brands fa-instagram px-2"></i>
            <i class="fa-brands fa-youtube px-2"></i>
        </div>
    </div>
    
  </header>
</template>

<script>
export default {
    name : 'BaseHeader'
}
</script>

<style lang="scss" scoped>
.header{
    background-color: var(--tertiary-color);
    color: var(--primary-color);
    max-width: 100%;

    .call{
         font-size: 12px;
        font-weight: 600;
    }

    .social{
        font-size: 14px;
    }
   

   
}
</style>