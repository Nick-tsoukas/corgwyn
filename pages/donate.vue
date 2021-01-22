<template>
  <div>
    <div class="w-full">
      <div class="relative shadow-xl sm:overflow-hidden">
        <div class="absolute inset-0">
          <img
            class="w-full h-full object-cover"
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
      class="pb-18 grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-4 mx-4 md:mx-16 lg:mx-28 xl:mx-32"
    >
      <div
        v-for="(source, i) in donateTo"
        :key="i"
        class="h-full w-full flex flex-col pt-8"
        :class="i === 0 && ` md:col-span-2 lg:col-span-1`"
      >
        <h2 class="text-3xl bold font-black text-corgiblue opacity-70">
          {{ source.title }}
        </h2>
        <p class="flex-grow text-gray-500 text-lg font-thin">
          {{ source.msg }}
        </p>
        <div class="mt-3">
          <button>
            <a
              :href="source.url"
              class="text-xl bg-green-400 text-white py-2 px-3 rounded-xl"
              >{{ source.btnTxt }}</a
            >
          </button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data: () => {
    return {
      donateTo: [
        {
          title: 'Donate with Venmo',
          url: 'https://venmo.com/LeAnne-Foust',
          msg: 'You can donate to CRS directly through Venmo.',
          btnTxt: 'Donate With Venmo',
        },
        {
          title: 'Amazon Wishlist',
          url: 'http://a.co/9sFiPPX',
          msg:
            'Check out our Amazon Wishlist – things wear out or get used up!',
          btnTxt: 'View Amazon Wishlist',
        },
        {
          title: 'PayPal',
          url: 'https://www.paypal.me/CorgwynRehab',
          msg: 'You can donate to CRS directly through PayPal.',
          btnTxt: 'Donate With PayPal',
        },
      ],
    }
  },
}
</script>
