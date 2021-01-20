<template>
  <div>
    <div
      class="rotate-180 overflow-hidden absolute w-full mx-auto -mt-10"
      style="transform: rotate(180deg)"
    >
      <svg
        style="height: 43px; width: 100%"
        class="block overflow-hidden"
        xmlns="http://www.w3.org/2000/svg"
        viewBox="0 0 1000 100"
        preserveAspectRatio="none"
      >
        <path class="" d="M500,98.9L0,6.1V0h1000v6.1L500,98.9z"></path>
      </svg>
    </div>
    <div
      class="grid grid-cols-1 md:grid-cols-2 items-center bg-black text-gray-100 px-10 md:px-16 py-24"
    >
      <!-- left -->
      <div class="">
        <h4>Corgwyn Rehabilitation Sanctuary</h4>
        <ul>
          <li class="">Jesup, IA</li>
          <li class="">(319) 849-8544</li>
          <li class="">corgwynrehab@gmail.com</li>
        </ul>
      </div>

      <!-- right -->
      <div>
        <ul>
          <li>
            <nuxt-link to="/"> Home </nuxt-link>
          </li>
          <li><nuxt-link to="/about"> About Us </nuxt-link></li>
          <li><nuxt-link to="/corgis">Our Corgis</nuxt-link></li>
          <li><nuxt-link to="/donate">Donate</nuxt-link></li>
          <li><nuxt-link to="/contact">Contact Us</nuxt-link></li>
          <li><a href="/sitemap.xml">HTML Sitemap</a></li>
        </ul>
      </div>
    </div>
    <div class="flex bg-corgiblue h-10 text-white px-10 items-center">
      <div>Corgwyn Rehabilitation Sanctuary © All Rights are Reserved</div>
      <div class="text-white ml-auto">
        <a href="https://www.facebook.com/CRSIowa/" target="_blank">
          <svg
            viewBox="0 0 512 512"
            xmlns="http://www.w3.org/2000/svg"
            class="w-6 h-6 ml-auto text-white"
          >
            <path
              fill="white"
              d="m512 256c0-141.4-114.6-256-256-256s-256 114.6-256 256 114.6 256 256 256c1.5 0 3 0 4.5-.1v-199.2h-55v-64.1h55v-47.2c0-54.7 33.4-84.5 82.2-84.5 23.4 0 43.5 1.7 49.3 2.5v57.2h-33.6c-26.5 0-31.7 12.6-31.7 31.1v40.8h63.5l-8.3 64.1h-55.2v189.5c107-30.7 185.3-129.2 185.3-246.1z"
            />
          </svg>
        </a>
      </div>
    </div>
  </div>
</template>

<script>
export default {}
</script>
