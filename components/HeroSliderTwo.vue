<template>
    <div class="intro-slider">
        <swiper :options="swiperOptions">
            <swiper-slide class="swiper-slide" v-for="(banner, index) in sliderData" :key="index">
<!--                <div class="intro-section overlay bg-cover" :style="{ backgroundImage: `url(${banner.bgImgSrc})` }">-->
<!--                    <div class="container">-->
<!--                        <div class="row row-cols-lg-1 row-cols-1">-->
<!--                            <div class="col align-self-center">-->
<!--                                <div class="intro-content m-auto text-center">-->
<!--                                    <h2 class="title">{{ banner.heading }}</h2>-->
<!--                                    <div class="desc">-->
<!--                                        <p>{{ banner.text }}</p>-->
<!--                                    </div>-->
<!--                                    <n-link to="/" class="btn btn-primary btn-hover-secondary">Get Started</n-link>-->
<!--                                    <n-link to="/" class="btn btn-outline-white btn-hover-primary">Learn More</n-link>-->
<!--                                </div>-->
<!--                            </div>-->
<!--                        </div>-->
<!--                    </div>-->
<!--                </div>-->
              <div class="video-background-holder">
                <div class="video-background-overlay"></div>
                <video playsinline="playsinline" autoplay="autoplay" muted="muted" loop="loop">
                  <source src="https://assets.mixkit.co/videos/preview/mixkit-man-working-on-his-laptop-308-large.mp4" type="video/mp4">
                </video>
                <div class="video-background-content container h-100">
                  <div class="d-flex h-100 text-center align-items-center">
                    <div class="intro-content m-auto text-white text-center">
                      <h2 class="title">{{ banner.heading }}</h2>
                      <div class="desc">
                        <p>
                          {{ banner.text }}
                        </p>
                      </div>
                      <n-link to="/" class="btn btn-primary btn-hover-secondary">Get Started</n-link>
                      <n-link to="/" class="btn btn-outline-white btn-hover-primary">Learn More</n-link>
                    </div>
                  </div>
                </div>
              </div>
            </swiper-slide>
        </swiper>
        <!-- pagination class -->
<!--        <div class="home-slider-prev swiper-button-prev main-slider-nav">-->
<!--            <i class="fal fa-angle-left"></i>-->
<!--        </div>-->
<!--        <div class="home-slider-next swiper-button-next main-slider-nav">-->
<!--            <i class="fal fa-angle-right"></i>-->
<!--        </div>-->
    </div>
</template>

<script>
    export default {
        data() {
            return {
                swiperOptions: {
                    speed: 1000,
                    loop: false,
                    autoplay: false,
                    spaceBetween : 30,
                    navigation: {
                        nextEl: '.swiper-button-next',
                        prevEl: '.swiper-button-prev',
                    },
                },

                sliderData: [
                    {
                        id: 1,
                        heading: "Impactful HR Software for Progressive Companies",
                        text: "IHUMANE is a customizable and comprehensive software that brings organization and effectiveness to the full range of Human Resource functions and responsibilities.",
                        bgImgSrc: "/images/hero-image/hero-3.jpg"
                    },
                    // {
                    //     id: 2,
                    //     heading: "Designing awesome brands & experiences",
                    //     text: "We are an agency located in New York. We think strategy, craft design, develop digital and create motion. To forward your brand and business.",
                    //     bgImgSrc: "/images/hero-image/hero-4.jpg"
                    // }
                ]
            }
        },
    };
</script>

<style>
/*
*
* ==========================================
* CUSTOM UTIL CLASSES
* ==========================================
*
*/

.video-background-holder {
  position: relative;
  background-color: black;
  height: calc(100vh);
  min-height: 25rem;
  width: 100%;
  overflow: hidden;
}

.video-background-holder video {
  position: absolute;
  top: 50%;
  left: 50%;
  min-width: 100%;
  min-height: 100%;
  width: auto;
  height: auto;
  z-index: 0;
  -ms-transform: translateX(-50%) translateY(-50%);
  -moz-transform: translateX(-50%) translateY(-50%);
  -webkit-transform: translateX(-50%) translateY(-50%);
  transform: translateX(-50%) translateY(-50%);
}

.video-background-content {
  position: relative;
  z-index: 2;
}

.video-background-overlay {
  position: absolute;
  top: 0;
  left: 0;
  height: 100%;
  width: 100%;
  background-color: black;
  opacity: 0.5;
  z-index: 1;
}

/*
*
* ==========================================
* FOR DEMO PURPOSES
* ==========================================
*
*/

code {
  padding: 0 0.15rem;
  background: #f5f5f5;
  border-radius: 0.2rem;
}
</style>
