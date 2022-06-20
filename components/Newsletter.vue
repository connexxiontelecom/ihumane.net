<template>
    <div class="section-padding-t110-b120 newsletter-section bg-cover" data-overlay="0.7" :style="{ backgroundImage: `url('/images/bg/newsletter.jpg')` }">
        <div class="container">
            <div class="row align-items-center">
                <div class="col-lg-12">
                    <div class="newsletter-content">
                        <SectionTitle
                          title="Get in touch with our team today."
                          sub-title="Want to learn how IHUMANE can help your organization?"
                          add-class-name="color-light"
                        />

                        <!-- Newsletter Form Start -->
                        <div class="newsletter-form">
                            <form>
                                <input type="email" placeholder="Enter your email" name="mail">
                                <button type="button" class="btn btn-primary btn-hover-secondary">Submit</button>
                            </form>
                        </div>
                        <!-- Newsletter Form End -->
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
