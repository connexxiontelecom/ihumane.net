<template>
    <div class="section-padding-t90-b100">
        <div class="container shape-animate">
            <!-- Section Title Start -->
            <SectionTitle title="Get In Touch" sub-title="Hi, want to get in touch? On this page, you'll find out how to reach us. We'd love to hear from you" add-class-name="mb-30" />
            <!-- Section Title End -->

            <div class="row row-cols-lg-3 row-cols-md-2 row-cols-sm-2 row-cols-1 mtn-30">
                <div class="col mt-30" data-aos="fade-up">
                    <div class="contact-info" data-vivus-hover>
                        <div class="icon">
                            <img class="svgInject" src="/images/svg/linea/linea-basic-map.svg" alt="Icon">
                        </div>
                        <div class="info">
                            <h4 class="title">Our Location</h4>
                            <span class="info-text">2A, Iller Crescent, Off Katsina Ala, Maitama, FCT Abuja, Nigeria</span>
                        </div>
                    </div>
                </div>

                <div class="col mt-30" data-aos="fade-up">
                    <div class="contact-info" data-vivus-hover>
                        <div class="icon">
                            <img class="svgInject" src="/images/svg/linea/linea-basic-message-txt.svg" alt="Icon">
                        </div>
                        <div class="info">
                            <h4 class="title">Give Us A Call</h4>
                            <span class="info-text"> +234 (0) 9 290 5141 <br> +234 (0) 901 640 0000</span>
                        </div>
                    </div>
                </div>

                <div class="col mt-30" data-aos="fade-up">
                    <div class="contact-info" data-vivus-hover>
                        <div class="icon">
                            <img class="svgInject" src="/images/svg/linea/linea-basic-mail-open-text.svg" alt="Icon">
                        </div>
                        <div class="info">
                            <h4 class="title">Help Desk</h4>
                            <span class="info-text">
                                <a href="mailto:info@ihumane.net">info@ihumane.net</a>
                                <br>
                                <a href="mailto:info@connexxiontelecom.com">info@connexxiontelecom.com</a>
                            </span>
                        </div>
                    </div>
                </div>
            </div>

            <shape-with-animation add-class-name="shape-1" data-depth="4" img-src="/images/shape-animation/video-shape-1.png" />

        </div>
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
