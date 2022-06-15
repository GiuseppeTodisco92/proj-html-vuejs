<template>
  <footer>
    <div class="footer-top py-5">
      <div class="container">
      <div class="row">
        <div class="col-3">
          <h5 class="py-2">about</h5>
          <p class="py-2">Lorem ipsum dolor sit amet consectetur adipisicing elit. Obcaecati mollitia deserunt temporibus, eveniet a provident doloribus et minima pariatur ducimus dicta quasi, quod quisquam eligendi. Cumque fugit aliquam natus ut.</p>
          <div><img src="../../assets/img/avada-movers-logo.png" alt="avada-movers-logo" class="logo_movers"></div>
        </div>
        <div class="col-4 px-5">
          <h5 class="py-2 ">avada movers</h5>
          <ul class="py-2">
            <li class="py-2" v-for="(linkAvada, index) in NavMovers" :key="index"><a :class="{active_green : linkAvada.current}" href="#" >{{linkAvada.link}}</a></li>
          </ul>
        </div>
        <div class="col-4 px-5">
          <h5 class="py-2 ">recent posts</h5>
          <ul class="py-2">
          <li class="py-2" v-for="(linkPosts, index) in NavRecentPosts" :key="index"><a  href="#">{{linkPosts.link}}</a></li>
          </ul>
        </div>
      </div>
    </div>
    </div>
    <div class="footer-bottom py-2 d-flex flex-column align-items-center">
      <div class="copyright py-3">
        <small>© copyright 2012 - 2020 | Avada Theme by ThemeFusion | All Rights Reserved | Powered by WordPress</small>
      </div>
      <div class="social">
            <i class="fa-brands fa-facebook-f px-2"></i>
            <i class="fa-brands fa-twitter px-2"></i>
            <i class="fa-brands fa-instagram px-2"></i>
            <i class="fa-brands fa-youtube px-2"></i>
        </div>

    </div>
    
  </footer>
</template>

<script>
export default {
    name: "BaseFooter",
    data(){
        return{
            TextButton: "free quote",
            NavMovers:[
                {
                    link: "Home",
                    current: true,
                },
                {
                    link: "Rates",
                    current: false,
                },
                {
                    link: "Testimonals",
                    current: false,
                },
               
                {
                    link: "Blog",
                    current: false,
                },
                {
                    link: "Free Quote",
                    current: false,
                },
            ],
            NavRecentPosts:[
                {
                    link: "Heading Out To College?",
                    current: true,
                },
                {
                    link: "Moving Your Business?",
                },
                {
                    link: "Outstanding Quality",
                },
               
                {
                    link: "Cost of moving",
                },
                {
                    link: "Best Moving Tips",
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
footer{
  background-color:var(--tertiary-color);
  padding-top: .9375rem;

  .footer-top{
    background-color:var(--primary-color);

    h5{
      font-weight: bold;
      font-size: 16px;
      text-transform: uppercase;
    }

    p{
      font-size: 12px;
    }

    ul{
      padding-left: 0rem;
    }

    li{
      list-style:none ;
      a{
        text-decoration: none;
        font-size: .75rem;
        color: var(--seventary-color);
      }
    }
    li:before{
      content: ">";
      font-size: .75rem;
      padding-right: .3125rem;
    }

    .active_green{
        color:var(--tertiary-color);
    }
  }

  .footer-bottom{
    color:var(--primary-color);
    font-size: .75rem;

    .social{
      padding-bottom: 1.25rem;
      font-size: 1.125rem;
    }
  }
   
}

</style>