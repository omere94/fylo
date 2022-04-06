<template>
  <section class="feature-list flex">
    <section v-for="(feature, idx) in features" :key="idx">
      <features-preview :item="feature" />
    </section>
  </section>
</template>

<script>
import featuresPreview from './featurePreview.vue'
export default {
  name: 'featuresList',
  components: {
    featuresPreview,
  },
  data() {
    return {
      features: [
        {
          img: '@/assets/img/icon-access-anywhere.svg',
          title: 'Access your files, anywhere',
          desc: 'The ability to use a smartphone, tablet, or computer to access your account means your files follow you everywhere.',
        },

        {
          img: '@/assets/img/icon-security.svg',
          title: 'Security you can trust',
          desc: '2-factor authentication and user-controlled encryption are just a couple of the security features we allow to help secure your files.',
        },

        {
          img: '@/assets/img/icon-collaboration.svg',
          title: 'Real-time collaboration',
          desc: 'Securely share files and folders with friends, family and colleagues for live collaboration. No email attachments required.',
        },

        {
          img: '@/assets/img/icon-any-file.svg ',
          title: 'Store any type of file',
          desc: "Whether you're sharing holidays photos or work documents, Fylo has you covered allowing for all file types to be securely stored and shared.",
        },
      ],
    }
  },
}
</script>

<style></style>
