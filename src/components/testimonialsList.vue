<template>
  <section class="test-list flex main-layout">
    <section v-for="(item, idx) in list" :key="idx">
      <testimonials-previewVue :item="item" />
    </section>
  </section>
</template>

<script>
import testimonialsPreviewVue from './testimonialsPreview.vue'
export default {
  name: 'testimonials',
  components: {
    testimonialsPreviewVue,
  },
  data() {
    return {
      list: [
        {
          img: '@/assets/img/profile-1.jpg',
          name: 'Satish Patel',
          position: 'Founder & CEO, Huddle',
          content:
            'Fylo has improved our team productivity by an order of magnitude. Since making the switch our team has become a well-oiled collaboration machine.',
        },
        {
          img: '@/assets/img/profile-2.jpg',
          name: 'Bruce McKenzie',
          position: 'Founder & CEO, Huddle',
          content:
            'Fylo has improved our team productivity by an order of magnitude. Since making the switch our team has become a well-oiled collaboration machine.',
        },
        {
          img: '@/assets/img/profile-3.jpg',
          name: 'Bruce McKenzie',
          position: 'Founder & CEO, Huddle',
          content:
            'Fylo has improved our team productivity by an order of magnitude. Since making the switch our team has become a well-oiled collaboration machine.',
        },
      ],
    }
  },
}
</script>

<style></style>
