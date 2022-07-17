<template>
  <div class="main-container">
    <TheHeader />

    <OffCanvasMobileMenu />

    <HeroSliderTwo />

    <AboutTwo />

    <FeatureOne :style="{ backgroundColor: '#f8faff' }" />

    <SkillWithVideo />

    <ContactSectionOne :style="{ backgroundColor: '#f8faff' }" />

    <TheFooter />
  </div>
</template>

<script>
export default {
  components: {
    TheHeader: () => import("@/components/TheHeader"),
    OffCanvasMobileMenu: () => import("@/components/OffCanvasMobileMenu"),
    SearchPopup: () => import("@/components/SearchPopup"),
    HeroSliderOne: () => import("@/components/HeroSliderOne"),
    HeroSliderTwo: () => import("@/components/HeroSliderTwo"),
    AboutOne: () => import("@/components/AboutOne"),
    AboutTwo: () => import("@/components/AboutTwo"),
    FeatureOne: () => import("@/components/FeatureOne"),
    SkillWithVideo: () => import("@/components/SkillWithVideo"),
    SuccessStory: () => import("@/components/SuccessStory"),
    PortfolioGallery: () => import("@/components/PortfolioGallery"),
    BlogSectionOne: () => import("@/components/BlogSectionOne"),
    Newsletter: () => import("@/components/Newsletter"),
    CallToActionOne: () => import("@/components/CallToActionOne"),
    ContactSectionOne: () => import("@/components/ContactSectionOne"),

    TheFooter: () => import("@/components/TheFooter"),
  },

  head() {
    return {
      title: "Home",
    };
  },
};
</script>
