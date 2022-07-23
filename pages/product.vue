<template>
  <div class="main-container">
    <TheHeader/>
    <OffCanvasMobileMenu/>
    <BreadcrumbOne
      :items="items"
      title="Product"
      backgroundUrl="/images/bg/rbg.jpeg"
    />
    <ProductOne/>
    <ProductTwo/>
    <ProductThree :style="{ backgroundColor: '#f8faff' }" />
    <CallToActionTwo />
    <ProductFour />
    <TheFooter />
  </div>
</template>

<script>
export default {
  components: {
    TheHeader: () => import("@/components/TheHeader"),
    OffCanvasMobileMenu: () => import("@/components/OffCanvasMobileMenu"),
    BreadcrumbOne: () => import("@/components/BreadcrumbOne"),
    ProductOne: () => import('@/components/ProductOne'),
    ProductTwo: () => import('@/components/ProductTwo'),
    ProductThree: () => import('@/components/ProductThree'),
    ProductFour: () => import('@/components/ProductFour'),
    CallToActionTwo: () => import('@/components/CallToActionTwo'),
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
          text: "Product",
          active: true,
        },
      ],
    };
  },
  head() {
    return {
      title: "Product",
    };
  },
}
</script>
