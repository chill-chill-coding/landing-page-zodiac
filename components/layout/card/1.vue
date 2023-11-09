<template>
  <img
    class="self-stretch h-1/4 rounded-[10px]"
    :src="`images/zodiacs/${zodiac.image}`" />
  <div
    class="self-stretch h-[193px] flex-col justify-start items-start gap-6 flex">
    <div
      class="self-stretch h-[137px] flex-col justify-start items-center gap-6 flex">
      <div
        class="self-stretch h-[65px] flex-col justify-start items-center flex">
        <div
          class="self-stretch text-neutral-800 text-2xl font-bold font-['Roboto'] uppercase leading-[33.60px]">
          {{ zodiac.title.toUpperCase() }}
        </div>
        <div
          class="self-stretch text-neutral-800 text-[22px] font-bold font-['Roboto'] leading-[30.80px]">
          {{ zodiac.date.toUpperCase() }}
        </div>
      </div>
      <div
        class="self-stretch text-neutral-800 text-base font-normal font-['Roboto'] leading-normal">
        {{ zodiac.detail }}
      </div>
    </div>
    <button
      class="self-stretch h-8 pt-2 flex-col justify-start items-start gap-2 flex">
      <div class="justify-center items-center gap-2 inline-flex">
        <div
          class="text-fuchsia-700 text-base font-normal font-['Roboto'] leading-normal">
          Explore All Horoscopes
        </div>
        <div class="w-6 h-6 relative"></div>
      </div>
    </button>
  </div>
</template>
<script setup>
const props = defineProps({
  zodiac: {
    type: Object,
    required: true,
  },
});
const { zodiac } = props;
</script>
<style lang=""></style>
