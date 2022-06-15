<template>
<div>
    <button>{{NameButton}}</button>
</div>
  
</template>

<script>
export default {
    name: "CustomButton",

    props:{
        NameButton: String,
    }
}
</script>

<style lang="scss" scoped>

    button{
        text-transform: uppercase;
        background-color: var(--secondary-color);
        color:var(--primary-color);
        font-size: .875rem;
        border-radius: 1.875rem;
        padding: .3125rem 1.5625rem;
        font-weight: bold;
        border: none;
    }
</style>