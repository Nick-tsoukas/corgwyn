<template>
  <div>
    <img src="/logo.png" alt="Corgwin logo image" class="py-8 pl-18" />
    <div
      class="pl-18 py-4 text-sm text-white bg-corgiblue"
      :class="scrollY >= 205 && 'navbar'"
    >
      <ul class="flex space-x-6 items-center justify-start">
        <li class="">HOME</li>
        <li class="">OUR CORGIS</li>
        <li class="">ABOUT US</li>
        <li class="">DONATE</li>
        <li class="">SPONSOR A CORGI</li>
        <li class="">CONTACT US</li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  data: () => {
    return {
      name: 'some mean man',
      scrollY: 0,
    }
  },
  mounted() {
    window.addEventListener('scroll', this.handleScroll)
  },
  methods: {
    handleScroll() {
      this.scrollY = window.scrollY
    },
  },
}
</script>

<style>
.navbar {
  position: fixed;
  top: 0;
  width: 100%;
}
</style>
