<template>
    <div class="section-padding-t90-b100">
        <div class="container">
            <!-- Section Title Start -->
            <SectionTitle
              title="We will help you retain and manage your employees"
              sub-title="You can focus on operations that really impact your company and leave the routine stuff to IHUMANE"
              add-class-name="mb-60"
            />
            <!-- Section Title End -->

            <div class="row row-cols-lg-3 row-cols-md-2 row-cols-sm-2 row-cols-1 mtn-30">
                <div class="col mt-30" data-aos="fade-up" v-for="(feature, index) in features" :key="index">
                    <div class="icon-box text-center" :class="addClassName">
                        <div class="icon">
                            <img class="svgInject" :src="feature.iconSrc" :alt="feature.title">
                        </div>
                        <div class="content">
                            <h3 class="title">{{ feature.title }}</h3>
                            <div class="desc">
                                <p>{{ feature.text }}</p>
                            </div>
                            <n-link to="/" class="link">Learn More</n-link>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        props: ["addClassName"],

        components: {
            SectionTitle: () => import("@/components/SectionTitle"),
        },

        data() {
            return {
                features: [
                    {
                        id: 1,
                        title: "Payroll Administration",
                        text: "Configure and perform the tasks necessary to organize employee compensation efficiently.",
                        iconSrc: "/images/svg/linea/linea-ecommerce-naira.svg"
                    },
                    {
                        id: 2,
                        title: "Employee Management",
                        text: "Perform the procedures that help measure, monitor, & interact with the workforce productively.",
                        iconSrc: "/images/svg/linea/linea-basic-book-pencil.svg"
                    },
                    {
                        id: 3,
                        title: "Biometrics Time Management",
                        text: "Transform outdated means of measuring employee time & attendance with innovative solutions.",
                        iconSrc: "/images/svg/linea/linea-basic-clock.svg"
                    },
                    {
                        id: 4,
                        title: "Employee Self-Service",
                        text: "Explore tools that decrease HR department workload through automation & paperwork elimination.",
                        iconSrc: "/images/svg/linea/linea-basic-elaboration-smartphone-cloud.svg"
                    },
                    {
                        id: 5,
                        title: "Real-Time Query & Chat",
                        text: "Engage employees more efficiently by sidestepping disincentives arising during communication.",
                        iconSrc: "/images/svg/linea/linea-basic-message-multiple.svg"
                    },
                    {
                        id: 5,
                        title: "Performance Management",
                        text: "Continuously improve performance by planning, assessing and developing employee skills. ",
                        iconSrc: "/images/svg/linea/linea-ecommerce-graph-increase.svg"
                    },
                ]
            }
        },
    };
</script>
