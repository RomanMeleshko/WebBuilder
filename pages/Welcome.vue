<template>
   <div id="Welcome">
      <div class="welcome">
         <div class="wrapper-welcome">
            <div class="container-fluid">
               <div class="row">

                  <div class="col-lg-6 col-md-12 text-lg-left text-md-center text-sm-center mt-lg-0 mt-md-4 left-block">
                     <div class="welcome-title">
                        <p class="title-one">WebBuilder</p>
                        <p class="title-two">Create your site dream</p>
                        <p class="title-three">Service for generater of simple templates for build html pages</p>
                        <div class="welcome-buttons">
                            <nuxt-link class="get_started btn btn-primary p-2" to="/Home">Get Started</nuxt-link>
                            <nuxt-link class="documentation btn btn-primary p-2" to="">Documentation</nuxt-link>
                        </div>
                     </div>

                  </div>
                  <div class="col-lg-6 col-md-0 right-block">

                     <swiper-container class="swiper mySwiper" ref="swiper">
                        <div class="swiper-wrapper">
                           <swiper-slide class="swiper-slide">
                              <img class="roboto_1" src="~/assets/images/welcome_page/roboto_copy_1.png" alt="roboto">
                           </swiper-slide>
                           <swiper-slide class="swiper-slide">
                              <img class="roboto_2" src="~/assets/images/welcome_page/roboto_copy_3.png" alt="roboto">
                           </swiper-slide>
                           <swiper-slide class="swiper-slide">
                              <img class="roboto_3" src="~/assets/images/welcome_page/roboto_copy_4.png" alt="roboto">
                           </swiper-slide>
                           <swiper-slide class="swiper-slide">
                              <img class="roboto_4" src="~/assets/images/welcome_page/roboto_copy_6.png" alt="roboto">
                           </swiper-slide>
                           <swiper-slide class="swiper-slide">
                              <img class="roboto_5" src="~/assets/images/welcome_page/roboto_copy_7.png" alt="roboto">
                           </swiper-slide>
                           <swiper-slide class="swiper-slide">
                              <img class="roboto_6" src="~/assets/images/welcome_page/roboto_copy_8.png" alt="roboto">
                           </swiper-slide>
                           <swiper-slide class="swiper-slide">
                              <img class="roboto_7" src="~/assets/images/welcome_page/roboto_copy_9.png" alt="roboto">
                           </swiper-slide>
                           <swiper-slide class="swiper-slide">
                              <img class="roboto_8" src="~/assets/images/welcome_page/roboto_copy_10.png" alt="roboto">
                           </swiper-slide>
                        </div>
                      </swiper-container>


                  </div>

               </div>

            </div>
         </div>

      </div>

   </div>
</template>

<script>
import Swiper from 'swiper/swiper-bundle.min';
import 'swiper/swiper-bundle.min.css';


 export default {
    name: "Welcome",
    data() {
       return {

      }
    },

    async mounted() {

       await this.$nextTick();
       new Swiper(this.$refs.swiper, {
          loop: true,
          effect: "flip",
          autoplay: {
             delay: 10000,
             disableOnInteraction: false,
          },
       });

    },

   layout: "welcome-empty"
 }
</script>

<style scoped>

.welcome {
  height: 100%;
  width: 100%;
  position: absolute;
  overflow: hidden;
  animation: move_background_colors 35s linear infinite;
  background: linear-gradient(149deg, rgba(24,187,156,0.7) 0%, rgba(106,57,175,0.5) 42%, rgba(187,24,148,0.3) 72%, rgba(115,53,134,0.1) 100%);
  background-size: 500%;
}

@keyframes move_background_colors {
   0% {
        background-position: 80% 0%;
    }
    50% {
        background-position: 20% 100%;
    }
    100% {
        background-position: 80% 0%;
    }
}

.welcome .right-block > img {
  position: relative;
  left: 10px;
}

.welcome-title > .title-one {
  font-size: 128px;
  font-weight: bold;
  color: #ffffff;
}
.welcome-title > .title-two {
  font-size: 24px;
  font-weight: 700;
  color: #ffffff;
}
.welcome-title > .title-three {
  font-size: 20px;
  font-weight: 700;
}

.welcome .welcome-buttons > .get_started,
.welcome .welcome-buttons > .documentation {
  width: 190px;
  margin-top: 50px;
  color: #333333;
  border: none;
  cursor: pointer;
}

.welcome .welcome-buttons > .get_started {
  background: #f36429;
}

.welcome .welcome-buttons > .documentation {
  background: #1baf4e;
  margin-left: 10px;
}

@media (min-width: 992px) and (max-width: 1800px) {

  .welcome-title {
    top: 200px;
    position: relative;
  }

  .welcome-title > .title-one {
    height: 70px;
    font-size: 73px;
  }

  .welcome-title > .title-two {
    font-size: 37px;

  }

  .welcome-title > .title-three {
    top: 40px;
    width: 390px;
    position: relative;
  }

  .welcome .welcome-buttons > button {
    width: 190px;
  }

  .swiper .roboto_1 {
    top: 50px;
    width: 560px;
    right: 25vw;
  }

  .swiper .roboto_2 {
    top: 40px;
    width: 560px;
    right: 25vw;
  }

  .swiper .roboto_3 {
    top: 30px;
    width: 500px;
    right: 25vw;
  }

  .swiper .roboto_4 {
    top: 40px;
    width: 560px;
    right: 27vw;
  }

  .swiper .roboto_5 {
    top: 40px;
    width: 560px;
    right: 25vw;
  }

  .swiper .roboto_6 {
    top: 30px;
    width: 560px;
    right: 25vw;
  }

  .swiper .roboto_7 {
    top: 90px;
    width: 560px;
    right: 26vw;
  }

  .swiper .roboto_8 {
    top: 130px;
    width: 450px;
    right: 370px;
  }

}

@media (min-width: 768px) and (max-width: 992px) {

  .welcome-title > .title-one {
    height: 95px;
    font-size: 103px;
  }

  .welcome-title > .title-two {
    font-size: 51px;
  }

  .welcome-title > .title-three {
    font-size: 17px;
    margin-top: 50px;
  }

  .welcome-title .welcome-buttons > button {
    width: 250px;
  }

  .swiper .roboto_1 {
    top: 30px;
    width: 560px;
    left: 50px;
  }

  .swiper .roboto_2 {
    top: 40px;
    right: 50px;
  }

  .swiper .roboto_3 {
    top: 30px;
    width: 560px;
  }

  .swiper .roboto_4 {
    top: 30px;
    right: 50px;
  }

  .swiper .roboto_5 {
    top: 30px;
    right: 20px;
  }

  .swiper .roboto_6 {
    right: 50px;
  }

  .swiper .roboto_7 {
    width: 560px;
  }

  .swiper .roboto_8 {
    width: 430px;
  }


}

@media (min-width: 576px) and (max-width: 768px) {

  .welcome-title > .title-one {
    height: 95px;
    font-size: 93px;
  }

  .welcome-title > .title-two {
    font-size: 46px;
  }

  .welcome-title > .title-three {
    font-size: 15px;
    margin-top: 50px;
  }

  .welcome-title .welcome-buttons > button {
    width: 220px;
  }

  .swiper .roboto_1 {
    top: 30px;
    width: 520px;
    left: 20px;
  }

  .swiper .roboto_2 {
    top: 40px;
    right: 50px;
    width: 500px;
  }

  .swiper .roboto_3 {
    top: 30px;
    width: 510px;
  }

  .swiper .roboto_4 {
    top: 30px;
    right: 20px;
    width: 500px;
  }

  .swiper .roboto_5 {
    top: 30px;
    width: 540px;
    right: 20px;
  }

  .swiper .roboto_6 {
    right: 20px;
    width: 570px;
  }

  .swiper .roboto_7 {
    width: 560px;
  }

  .swiper .roboto_8 {
    top: 50px;
    width: 400px;
  }

}

@media (min-width: 320px) and (max-width: 576px) {

  .welcome-title > .title-one {
    height: 60px;
    text-align: center;
    font-size: 63px;
  }

  .welcome-title > .title-two {
    text-align: center;
    font-size: 32px;
  }

  .welcome-title > .title-three {
    text-align: center;
    font-size: 15px;
    margin-top: 50px;
  }

  .welcome-title .welcome-buttons > .get_started,
  .welcome-title .welcome-buttons > .documentation {
    width: 130px;
  }

  .welcome-title .welcome-buttons {
    text-align: center;
  }

  .welcome .left-block {
    margin-top: 20px;
  }

  .swiper .roboto_1 {
    top: 20px;
    width: 70vw;
    left: 10px;
  }

  .swiper .roboto_2 {
    top: 20px;
    right: 10px;
    width: 70vw;
  }

  .swiper .roboto_3 {
    top: 20px;
    width: 70vw;
  }

  .swiper .roboto_4 {
    top: 20px;
    right: 20px;
    width: 70vw;
  }

  .swiper .roboto_5 {
    top: 20px;
    width: 90vw;
    right: 20px;
  }

  .swiper .roboto_6 {
    top: 10px;
    right: 20px;
    width: 90vw;
  }

  .swiper .roboto_7 {
    top: 10px;
    right: 20px;
    width: 80vw;
  }

  .swiper .roboto_8 {
    top: 10px;
    right: 20px;
    width: 80vw;
  }


}

  .swiper {
    width: 100vw;
    height: 100vh;
  }

  .swiper-slide {
    text-align: center;
    font-size: 18px;
  }

  .swiper img {
    position: relative;
  }

</style>
