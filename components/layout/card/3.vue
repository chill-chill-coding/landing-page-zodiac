<template lang="">
  <img class="self-stretch h-full rounded-[10px]" :src="`images/accessories/${accessory.image}`" />
  <div class="self-stretch h-full flex-col justify-start items-start gap-6 flex">
      <div class="self-stretch h-[195px] flex-col justify-start items-center gap-6 flex">
          <div class="self-stretch h-[99px] flex-col justify-start items-center flex">
              <div class="self-stretch text-neutral-800 text-2xl font-bold font-['Roboto'] uppercase leading-[33.60px]">{{accessory.header}}</div>
              <div class="self-stretch text-neutral-800 text-[22px] font-normal font-['Roboto'] leading-[30.80px]">${{accessory.price}}</div>
          </div>
          <div class="self-stretch text-neutral-800 text-base font-normal font-['Roboto'] leading-normal">{{accessory.detail}}</div>
      </div>
      <button class="self-stretch h-8 pt-2 flex-col justify-start items-start gap-2 flex">
          <div class="justify-center items-center gap-2 inline-flex">
              <div class="text-fuchsia-700 text-base font-normal font-['Roboto'] leading-normal">Shop now</div>
              <div class="w-6 h-6 relative"></div>
          </div>
      </button>
  </div>
</template>
<script setup>
const props = defineProps({
  accessory: {
    type: Object,
    required: true,
  },
});
const { accessory } = props;
</script>
