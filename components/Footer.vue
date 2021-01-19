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
    <div class="bg-corgiblue h-8">bottom</div>
  </div>
</template>

<script>
export default {}
</script>
