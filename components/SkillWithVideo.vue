<template>
    <div class="section-padding">
        <div class="container">
            <div class="row align-items-center">
                <div class="col-xl-5 col-lg-6 col-12" data-aos="fade-up">
                    <div class="skill-with-video-content">
                        <!-- Section Title Two Start -->
                        <div class="section-title-two">
                            <span class="sub-title">Why choose our service?</span>
                            <h3 class="title">
                              <a href="https://connexxiontelecom.com" target="_blank">Connexxion Telecom & Solutions</a> is a provider of core IT networking, communication services,
                              and software solutions. We work with you to understand your unique business objectives
                              which allows us to innovate your business models to reduce operational costs.
                            </h3>
                        </div>
                        <!-- Section Title Two End -->

                        <!-- Agency List Start -->
                        <ul class="agency-list">
                            <li class="item">
                                <div class="icon">
                                    <i class="fas fa-check"></i>
                                </div>
                                <div class="text">Proudly Nigerian 🇳🇬</div>
                            </li>
                            <li class="item">
                                <div class="icon">
                                    <i class="fas fa-check"></i>
                                </div>
                                <div class="text">Configurable to your specifications</div>
                            </li>
                            <li class="item">
                                <div class="icon">
                                    <i class="fas fa-check"></i>
                                </div>
                                <div class="text">24/7 customer support</div>
                            </li>
                            <li class="item">
                                <div class="icon">
                                    <i class="fas fa-check"></i>
                                </div>
                                <div class="text">Data privacy, integrity and security</div>
                            </li>
                        </ul>
                        <!-- Agency List End -->
                        <n-link to="/contact-us" class="btn btn-primary btn-hover-secondary">
                            Get started for free
                        </n-link>
                    </div>
                </div>

                <div class="offset-xl-1 col-xl-6 col-lg-6 col-12">
                    <div class="video-popup-area">
                        <div class="skill-video">
                            <client-only>
                                <silent-box :image="videos[0]">
                                    <template v-slot:silentbox-item>
                                        <img class="image" src="/images/video/skill-video-1.jpg" alt="image" />
                                        <div class="icon video-popup">
                                            <i class="fas fa-play"></i>
                                        </div>
                                    </template>
                                </silent-box>
                            </client-only>
                        </div>

                        <!-- Animation Shape Start -->
                        <ShapeWithAnimation addClassName="shape-1" data-depth="1" imgSrc="/images/shape-animation/video-shape-1.png" />
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    components: {
        ShapeWithAnimation: () => import("@/components/ShapeWithAnimation")
    },

    data() {
        return {
            videos: [
                {
                    src: "https://www.youtube.com/watch?v=VT5vhtSL1BA&ab_channel=ConnexxionTelecoms"
                }
            ]
        };
    }
};
</script>
