<template>
  <div class="main-container">
    <TheHeader />
    <OffCanvasMobileMenu />
    <BreadcrumbOne
      :items="items"
      title="Contact Us"
      backgroundUrl="/images/bg/rbg.jpeg"
    />
    <CallToActionOne />
    <!--Google Map Area Start-->
    <div class="google-map-area section-padding-bottom">
      <div class="container">
        <div class="contact-map-area">
          <iframe class="contact-map" src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3939.661137981724!2d7.4915712299365165!3d9.09460116960626!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x104e0bbeb16a3f9b%3A0x50d5084bb4bc3f5e!2sConnexxion%20Telecom%20and%20Solutions!5e0!3m2!1sen!2sng!4v1658606528984!5m2!1sen!2sng" width="600" height="450" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
        </div>
      </div>
    </div>
    <!--Google Map Area Start-->
    <ContactForm />
    <TheFooter />
  </div>
</template>

<script>
export default {
  components: {
    TheHeader: () => import("@/components/TheHeader"),
    OffCanvasMobileMenu: () => import("@/components/OffCanvasMobileMenu"),
    BreadcrumbOne: () => import("@/components/BreadcrumbOne"),
    CallToActionOne: () => import('@/components/CallToActionOne'),
    ContactForm: () => import('@/components/ContactForm'),
    TheFooter: () => import("@/components/TheFooter"),
  },
  data() {
    return {
      items: [
        {
          text: "Home",
          to: "/",
        },
        {
          text: "Contact Us",
          active: true,
        },
      ],
    };
  },
  head() {
    return {
      title: "Contact Us",
    };
  },
}
</script>
