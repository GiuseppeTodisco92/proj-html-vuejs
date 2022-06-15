<template>

  <section>

    <div class="container d-flex justify-content-between align-items-center py-2">
        <div><img src="../../assets/img/avada-movers-logo.png" alt="avada-movers-logo" class="logo_movers"></div>
        <nav class="d-flex align-items-center">
            <ul class="d-flex ">
                <li class="d-flex mx-4" v-for="(link, index) in NavLink" :key="index"  ><a :class="{active_green : link.current}" class="link_style" href="#">{{link.link}}</a></li>
            </ul>
            <a href="#"><custom-button :NameButton="TextButton"/></a>
        </nav>
        
    </div>

    <div class="hero_text container d-flex flex-column justify-content-center align-items-center ">
        <small>moving without the hassle</small>
        <h1>we make it simple</h1>
        <small>professional service with quality and customer satisfaction</small>
    </div>

    <div class="hero_footer">
        <h6><i class="fa-solid fa-paper-plane px-2"></i>get a free quote online now!</h6>
    </div>

  </section>

</template>

<script>
import CustomButton from '../Commons/CustomButton.vue'
export default {
  
    name: "SectionHero",
    components: { 
        CustomButton
         },

    data(){
        return{
            TextButton: "free quote",
            NavLink:[
                {
                    link: "Home",
                    current: true,
                },
                {
                    link: "Rates",
                },
                {
                    link: "Testimonals",
                },
                {
                    link: "FAQ",
                },
                {
                    link: "Blog",
                },
                {
                    link: "Contact",
                },
                

            ]
        }
    }
}
</script>

<style lang="scss" scoped>
section{
    background-image: url("../../assets/img/avada-movers-homeherobackground-final.jpg");
    background-size: cover;
    .logo_movers{
        width: 7.5rem;
    }

    .hero_text{
    height: 34rem;
    text-transform: uppercase;
    font-weight:900;
    }
    
    small{
        color:var( --sixtary-color);
    }
    h1{
        font-weight: bold;
        font-size: 58px;
    }
    ul{
        margin-top: 14px;
        
    }
    .link_style{
        text-decoration: none;
        color:var(--seventary-color);
        font-weight: bold;
    }

    .active_green{
        color:var(--tertiary-color);
    }

    a:hover{
        color:var(--tertiary-color);
    }

    .hero_footer{
        display:flex;
        justify-content: center;
        align-items: center;
        padding: 40px 0px;
        background-color: var(--secondary-color);
        color:var(--primary-color);

        h6{
            text-transform: uppercase;
            font-size:14px;
            letter-spacing: 2px;
        }
    }
}

</style>