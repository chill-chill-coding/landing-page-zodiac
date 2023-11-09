<template lang="">
  <div
    class="grow shrink basis-0 self-stretch flex-col justify-center items-end inline-flex">
    <img
      class="self-stretch h-full rounded-tl-[10px] rounded-bl-[10px]"
      :src="`images/zodiacs/${period.image}`" />
  </div>
  <div
    class="grow shrink basis-0 self-stretch p-6 flex-col justify-center items-start gap-6 inline-flex">
    <div
      class="self-stretch h-[114px] flex-col justify-start items-start gap-2 flex">
      <div
        class="self-stretch h-[114px] flex-col justify-start items-start gap-2 flex">
        <div
          class="self-stretch text-neutral-800 text-2xl font-bold font-['Roboto'] leading-[33.60px]">
          {{period.header}}
        </div>
        <div
          class="self-stretch text-neutral-800 text-base font-normal font-['Roboto'] leading-normal">
          {{period.detail}}
        </div>
      </div>
    </div>
    <button class="self-stretch justify-start items-center gap-6 inline-flex">
      <div class="justify-center items-center gap-2 flex">
        <div
          class="text-fuchsia-700 text-base font-normal font-['Roboto'] leading-normal">
          Dive Deeper into the Cosmos
        </div>
        <div class="w-6 h-6 relative"></div>
      </div>
    </button>
  </div>
</template>
<script setup>
const props = defineProps({
  period: {
    type: Object,
    required: true,
  },
});
const { period } = props;
</script>
