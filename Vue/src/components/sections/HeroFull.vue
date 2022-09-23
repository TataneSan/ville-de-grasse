<template>
    <section
        class="hero section center-content"
        :class="[
            hasBgColor && 'has-bg-color',
            invertColor && 'invert-color'
        ]">
        <div class="container-sm">
            <div
                class="hero-inner section-inner"
                :class="[
                    topDivider && 'has-top-divider',
                    bottomDivider && 'has-bottom-divider'
                ]">
                <div class="hero-content">
                    <h1 class="mt-0 mb-16 reveal-from-bottom" data-reveal-delay="200">
                        Landing template for startups
                    </h1>
                    <div class="container-xs">
                        <p class="m-0 mb-32 reveal-from-bottom" data-reveal-delay="400">
                            Our landing page template works on all devices, so you only have to set it up once, and get beautiful results forever.
                        </p>
                        <div class="reveal-from-bottom" data-reveal-delay="600">
                            <c-button tag="a" color="primary" href="https://cruip.com/">
                                Get started
                            </c-button>
                        </div>
                    </div>
                </div>
                <div class="hero-figure illustration-element-01 reveal-from-bottom" data-reveal-value="20px" data-reveal-delay="800">
                    <c-image
                        class="has-shadow"
                        :src="require('@/assets/images/hero-image.png')"
                        alt="Hero"
                        :width="896"
                        :height="504" />
                </div>
            </div>
        </div>
    </section>
</template>

<script>
import { SectionProps } from '@/utils/SectionProps.js'
import CButton from '@/components/elements/Button.vue'
import CImage from '@/components/elements/Image.vue'

export default {
  name: 'CHeroFull',
  mixins: [SectionProps],
  components: {
    CButton,
    CImage
  }
}
</script>