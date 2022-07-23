<template>
  <div class="main-container">
    <TheHeader />
    <OffCanvasMobileMenu />
    <BreadcrumbOne
      :items="items"
      title="Appreciation"
      backgroundUrl="/images/bg/rbg.jpeg"
    />
    <CallToActionThree />
    <TheFooter />
  </div>
</template>

<script>
export default {
  components: {
    TheHeader: () => import("@/components/TheHeader"),
    OffCanvasMobileMenu: () => import("@/components/OffCanvasMobileMenu"),
    BreadcrumbOne: () => import("@/components/BreadcrumbOne"),
    CallToActionThree: () => import("@/components/CallToActionThree"),
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
          text: "Appreciation",
          active: true,
        },
      ],
    };
  },
  head() {
    return {
      title: "Appreciation",
    };
  },
};
</script>
