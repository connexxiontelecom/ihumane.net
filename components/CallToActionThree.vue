<template>
  <div class="cta-section section-padding-t90-b100">
    <div class="container text-center icon-up-down-animation">
      <!-- Section Title Start -->
      <div class="section-title text-center" data-aos="fade-up">
        <h2 class="title fz-34">Thank you for signing up on IHUMANE.</h2>
        <p class="sub-title">
          Because we respect your privacy and are compliant with the global anti-spamming regulations, here’s what you
          can expect from us:
        </p>
        <div class="text mt-3">
          <i class="fas fa-check mr-2 text-primary"></i>
          A welcoming email that should be sitting pretty in your mailbox already.
        </div>
        <div class="text">
          <i class="fas fa-check mr-2 text-primary"></i>
          Gift items in form of business e-books and nuggets.
        </div>
        <div class="text">
          <i class="fas fa-check mr-2 text-primary"></i>
          IHUMANE and complementary product related information.
        </div>
        <div class="text">
          <i class="fas fa-check mr-2 text-primary"></i>
          Newsletters and Product update alerts you will find useful for business and upgrades.
        </div>
        <p class="mt-3 sub-title">
          If you’d like us to demonstrate how IHUMANE works for you over a brief live session, please schedule a call
          <a href="javascript:void(0)" class="font-weight-bolder" target="_blank">here</a>.
        </p>
      </div>
      <!-- Section Title End -->
      <a
        href="https://app.ihumane.net/login"
        class="btn btn-primary btn-hover-secondary"
      >
        Continue to IHUMANE App
      </a>
<!--      <a href="javascript:void(0)" class="btn btn-outline-primary btn-hover-primary">-->
<!--        Book a Demo-->
<!--      </a>-->

      <!-- Icon Animation Start -->
      <!--      <div-->
      <!--        class="shape"-->
      <!--        v-for="(shape, index) in shapeData"-->
      <!--        :key="index"-->
      <!--        :class="shape.className"-->
      <!--      >-->
      <!--        <span>-->
      <!--          <img :src="shape.imgSrc" alt="icon" />-->
      <!--        </span>-->
      <!--      </div>-->
      <!-- Icon Animation End -->
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      shapeData: [
        {
          imgSrc: "/images/icon-animation/icon-1.png",
          className: "shape-1",
        },
        {
          imgSrc: "/images/icon-animation/icon-2.png",
          className: "shape-2",
        },
        {
          imgSrc: "/images/icon-animation/icon-3.png",
          className: "shape-3",
        },
        {
          imgSrc: "/images/icon-animation/icon-4.png",
          className: "shape-4",
        },
        {
          imgSrc: "/images/icon-animation/icon-5.png",
          className: "shape-5",
        },
        {
          imgSrc: "/images/icon-animation/icon-6.png",
          className: "shape-6",
        },
        {
          imgSrc: "/images/icon-animation/icon-7.png",
          className: "shape-7",
        },
        {
          imgSrc: "/images/icon-animation/icon-8.png",
          className: "shape-8",
        },
        {
          imgSrc: "/images/icon-animation/icon-9.png",
          className: "shape-9",
        },
      ],
    };
  },
};
</script>
