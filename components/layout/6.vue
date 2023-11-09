<template>
    <div class="w-full h-11/12 px-16 py-28 bg-white justify-center items-start gap-12 inline-flex">
        <div class="w-[768px] flex-col justify-start items-center gap-20 inline-flex">
            <div class="h-[58px] flex-col justify-start items-start gap-6 flex">
                <div class="self-stretch text-center text-neutral-800 text-5xl font-bold font-['Roboto'] leading-[57.60px]">Frequently asked questions</div>
            </div>
            <div class="self-stretch h-[366px] flex-col justify-start items-start flex">
                <div v-for="(question, index) in questions" :key="index" class="self-stretch h-[73px] flex-col justify-start items-start flex">
                    <LayoutDropdown1 :question="question"/>
                </div>
               
            </div>
            <div class="h-[157px] flex-col justify-start items-center gap-6 flex">
                <div class="self-stretch h-[85px] flex-col justify-start items-center gap-4 flex">
                    <div class="self-stretch text-center text-neutral-800 text-[32px] font-bold font-['Roboto'] leading-[41.60px]">Still have questions?</div>
                    <div class="self-stretch text-center text-neutral-800 text-lg font-normal font-['Roboto'] leading-[27px]">Support details to capture customers that might be on the fence.</div>
                </div>
                <button class="px-6 py-3 border border-fuchsia-700 justify-center items-center gap-2 inline-flex">
                    <div class="text-fuchsia-700 text-base font-normal font-['Roboto'] leading-normal">Contact us</div>
                </button>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    data() {
        return {
            questions: [
                {question:"How do I find my daily horoscope?"},
                {question:"Can I buy zodiac accessories for a friend as a gift?"},
                {question:"How does the AI Matching for horoscopes work?"},
                {question:"Is it safe to shop on this website?"},
                {question:"How often are the horoscopes updated?"}
            ]
        }
    }
}
</script>
<style lang="">
    
</style>