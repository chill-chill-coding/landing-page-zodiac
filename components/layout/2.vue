<template>
  <div
    class="w-full h-11/12 px-16 py-28 bg-white flex-col justify-start items-center gap-20 inline-flex">
    <div class="h-12 flex-col justify-start items-center gap-4 flex">
      <div
        class="self-stretch h-12 flex-col justify-start items-center gap-6 flex">
        <div
          class="self-stretch text-center text-neutral-800 text-[40px] font-bold font-['Roboto'] uppercase leading-[48px]">
          Monthly and Yearly Horoscopes
        </div>
      </div>
    </div>
    <div
      class="self-stretch h-80 flex-col justify-start items-start gap-8 flex">
      <div class="self-stretch justify-start items-start gap-8 inline-flex">
        <div
          v-for="period in periods"
          class="grow shrink basis-0 h-80 bg-white rounded-[10px] border border-neutral-800 border-opacity-50 justify-start items-start flex">
          <LayoutCard2 :period="period" />
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      periods: [
        {
          header: "Monthly Horoscopes",
          detail:
            "Plan ahead and align your energies with the cosmos with our insightful monthly horoscopes.",
          image: "image 20.png",
        },
        {
          header: "Yearly Horoscopes",
          detail:
            "Embark on a journey of self-discovery and prepare for the year ahead with our comprehensive yearly insights.",
          image: "image 21.png",
        },
      ],
    };
  },
};
</script>
<style lang=""></style>
