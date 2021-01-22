<template>
  <div>
    <div class="w-full">
      <div class="relative shadow-xl sm:overflow-hidden">
        <div class="absolute inset-0">
          <img
            class="h-full w-full object-cover"
            src="/corgis-home.jpeg"
            alt="People working with corgis"
          />
          <div
            class="absolute inset-0 bg-gradient-to-r from-gray-600 to-gray-500"
            style="mix-blend-mode: multiply"
          ></div>
        </div>
        <div class="relative px-4 py-16 sm:px-6 sm:py-24 lg:py-32 lg:px-8">
          <h1
            class="text-corgiblue text-center text-4xl font-extrabold tracking-tight sm:text-5xl lg:text-6xl"
          >
            Help Keep CRS Thriving!
          </h1>
          <p
            class="mt-6 max-w-lg mx-auto text-center text-xl text-indigo-200 sm:max-w-3xl"
          >
            Help Keep CRS Thriving! Corgwyn Rehabilitation Sacntuary is now
            officially a 501(c)(3)! This means all donations are tax deductible.
            We offer several forms of donation, including cash donations, corgi
            sponsorships, and an Amazon wishlist.
          </p>
        </div>
      </div>
    </div>

    <!-- donate section -->
    <div
      class="pt-8 pb-14 grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-4 mx-4 md:mx-16 lg:mx-40"
    >
      <div class="bg-red-800 h-40 w-full md:col-span-2 lg:col-span-1">
        <h2>Donate with Venmo</h2>
      </div>
      <div class="bg-red-800 h-40 w-full">
        <h2>Amazon Wishlist</h2>
      </div>
      <div class="bg-red-800 h-40 w-full">
        <h2>Donate with PayPal</h2>
      </div>
    </div>
  </div>
</template>

<script>
export default {}
</script>
