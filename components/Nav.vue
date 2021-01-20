<template>
  <div>
    <img src="/logo.png" alt="Corgwin logo image" class="py-8 pl-18" />
    <div
      class="pl-18 py-4 text-sm text-white bg-corgiblue"
      :class="scrollY >= 205 && 'navbar'"
    >
      <ul class="flex space-x-6 items-center justify-start">
        <li class=""><nuxt-link to="/">HOME</nuxt-link></li>
        <li class=""><nuxt-link to="/our-corgis">OUR CORGIS</nuxt-link></li>
        <li class=""><nuxt-link to="/about">ABOUT US</nuxt-link></li>
        <li class=""><nuxt-link to="/donate">DONATE</nuxt-link></li>
        <li class=""><nuxt-link to="/sponsor">SPONSOR A CORGI</nuxt-link></li>
        <li class=""><nuxt-link to="/contact">CONTACT US</nuxt-link></li>
      </ul>
    </div>
    <button
      v-show="scrollY >= 400"
      @click="scrollToTop"
      class="w-12 h-12 fixed bottom-0 right-0 mb-10 mr-10 text-white bg-black rounded-full"
    >
      <svg
        xmlns="http://www.w3.org/2000/svg"
        class="w-8 ml-3 pl-1"
        viewBox="0 0 512 512"
      >
        <path
          fill="currentColor"
          d="M88 166.059V468c0 6.627 5.373 12 12 12h56c6.627 0 12-5.373 12-12V166.059h46.059c21.382 0 32.09-25.851 16.971-40.971l-86.059-86.059c-9.373-9.373-24.569-9.373-33.941 0l-86.059 86.059c-15.119 15.119-4.411 40.971 16.971 40.971H88z"
        />
      </svg>
    </button>
  </div>
</template>

<script>
export default {
  data: () => {
    return {
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
    scrollToTop() {
      window.scrollTo(0, 0)
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
