<template>
  <div>
    <div class="w-[768px] h-px bg-neutral-800"></div>
    <div class="w-[768px] py-5 justify-start items-center gap-3 inline-flex">
      <div
        class="grow shrink basis-0 text-neutral-800 text-lg font-bold font-['Roboto'] leading-[27px]">
        {{ question.question }}
      </div>
      <button class="w-8 h-8 relative">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          fill="none"
          viewBox="0 0 24 24"
          strokeWidth="{1.5}"
          stroke="currentColor"
          className="w-6 h-6">
          <path
            strokeLinecap="round"
            strokeLinejoin="round"
            d="M19.5 8.25l-7.5 7.5-7.5-7.5" />
        </svg>
      </button>
    </div>
  </div>
</template>
<script setup>
const props = defineProps({
  question: {
    type: Object,
    required: true,
  },
});
const { question } = props;
console.log(question);
</script>
