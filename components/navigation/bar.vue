<template>
  <div
    class="w-full h-20 px-16 bg-white shadow-inner flex-col justify-center items-center inline-flex">
    <div class="self-stretch justify-between items-center inline-flex">
      <nuxt-link to="/" class="justify-start items-start flex">
        <div class="w-16 h-7 relative">
          <img src="/images/logo.png"/>
        </div>
      </nuxt-link>
      <div class="bg-white justify-center items-center gap-8 flex">
        <div class="justify-start items-start gap-8 flex">
          <div
            class="text-neutral-800 text-base font-normal font-['Roboto'] leading-normal">
            Home
          </div>
          <div
            class="text-neutral-800 text-base font-normal font-['Roboto'] leading-normal">
            Daily Horoscope
          </div>
          <div
            class="text-neutral-800 text-base font-normal font-['Roboto'] leading-normal">
            Monthly Horoscope
          </div>
          <div
            class="text-neutral-800 text-base font-normal font-['Roboto'] leading-normal">
            Yearly Horoscope
          </div>
          <div
            class="text-neutral-800 text-base font-normal font-['Roboto'] leading-normal">
            Zodiac Accessories
          </div>
          <div
            class="text-neutral-800 text-base font-normal font-['Roboto'] leading-normal">
            Fortune Teller
          </div>
          <div
            class="text-neutral-800 text-base font-normal font-['Roboto'] leading-normal">
            Contact
          </div>
        </div>
        <div class="justify-center items-center gap-4 flex">
          <div class="px-5 py-2 border border-fuchsia-700 justify-center items-center gap-2 flex">
            <button
              class="text-fuchsia-700 text-base font-normal font-['Roboto'] leading-normal">
              Sign In
            </button>
          </div>
          <div
            class="px-5 py-2 bg-fuchsia-700 border border-fuchsia-700 justify-center items-center gap-2 flex">
            <button
              class="text-white text-base font-normal font-['Roboto'] leading-normal">
              Join Now
            </button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  methods: {
    showAlert: () => {
      alert("this is a logo")
    }
  }
};
</script>
<style lang="ts"></style>
