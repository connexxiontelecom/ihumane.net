<template>
    <div class="section-padding-t110-b120 newsletter-section bg-cover-top" data-overlay="0.7" :style="{ backgroundImage: `url('/images/bg/product.jpeg')` }">
        <div class="container">
            <div class="row align-items-center">
                <div class="col-lg-12">
                    <div class="cta-content text-center">
                        <SectionTitle
                          title="Interested in IHUMANE?"
                          sub-title="There has never been an easier way to automate all your HR processes!"
                          add-class-name="color-light"
                        />
                        <a href="#" class="btn btn-primary btn-hover-secondary mt-6">Get Started For Free</a>
                    </div>
                </div>
            </div>
        </div>
        <ShapeWithAnimation add-class-name="shape-1" data-depth="1" img-src="/images/shape-animation/newsletter-shape.png" />
    </div>
</template>

<script>
    export default {
        components: {
            SectionTitle: () => import("@/components/SectionTitle"),
            ShapeWithAnimation: () => import("@/components/ShapeWithAnimation"),
        },
    };
</script>
