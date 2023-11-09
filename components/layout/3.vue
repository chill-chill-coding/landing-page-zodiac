<template>
    <div class="w-full h-11/12 px-16 py-28 bg-white justify-start items-center gap-20 inline-flex">
        <div class="grow shrink basis-0 flex-col justify-start items-start gap-8 inline-flex">
            <div class="self-stretch h-[450px] flex-col justify-start items-start gap-10 flex">
                <div class="self-stretch h-[126px] flex-col justify-start items-start gap-6 flex">
                    <div class="self-stretch text-neutral-800 text-[40px] font-bold font-['Roboto'] uppercase leading-[48px]">AI Matching</div>
                    <div class="self-stretch text-neutral-800 text-lg font-normal font-['Roboto'] leading-[27px]">Discover your celestial counterpart and enhance your zodiac journey with our cutting-edge AI horoscope matching.</div>
                </div>
                <div class="self-stretch justify-start items-start gap-6 inline-flex">
                    <div class="grow shrink basis-0 flex-col justify-start items-start gap-4 inline-flex">
                        <div class="self-stretch text-neutral-800 text-2xl font-bold font-['Roboto'] leading-[33.60px]">Personalized Matches</div>
                        <div class="self-stretch text-neutral-800 text-base font-normal font-['Roboto'] leading-normal">Find your perfect horoscope match for deeper connections and understanding</div>
                        <button class="self-stretch h-8 pt-2 flex-col justify-start items-start gap-2 flex">
                            <div class="justify-center items-center gap-2 inline-flex">
                                <div class="text-fuchsia-700 text-base font-normal font-['Roboto'] leading-normal">Learn more</div>
                                <div class="w-6 h-6 relative"></div>
                            </div>
                        </button>
                    </div>
                </div>
                <div class="self-stretch justify-start items-start gap-6 inline-flex">
                    <div class="grow shrink basis-0 flex-col justify-start items-start gap-4 inline-flex">
                        <div class="self-stretch text-neutral-800 text-2xl font-bold font-['Roboto'] leading-[33.60px]">Zodiac Empowerment</div>
                        <div class="self-stretch text-neutral-800 text-base font-normal font-['Roboto'] leading-normal">Curated items that resonate with your star sign, enhancing your cosmic vibrations</div>
                        <button class="self-stretch h-8 pt-2 flex-col justify-start items-start gap-2 flex">
                            <div class="justify-center items-center gap-2 inline-flex">
                                <div class="text-fuchsia-700 text-base font-normal font-['Roboto'] leading-normal">Learn more</div>
                                <div class="w-6 h-6 relative"></div>
                            </div>
                        </button>
                    </div>
                </div>
            </div>
            <button class="pt-4 justify-start items-center gap-6 inline-flex">
                <div class="px-6 py-3 border border-fuchsia-700 justify-center items-center gap-2 flex">
                    <div class="text-fuchsia-700 text-base font-normal font-['Roboto'] leading-normal">Unlock Your Celestial Harmony</div>
                </div>
            </button>
        </div>
        <img class="grow shrink basis-0 h-[640px] rounded-[10px]" src="images/image 22.png" />
    </div>
</template>
<script>
export default {
    data() {
        return {
            accessories: [
                {
                    title: "Aries Zodiac Charm Bracelet",
                    price: "$29.99",
                    detail: "Energetic leaders, passionate and adventurous, with a love for challenges.",
                    image: "image 5.png"
                },
            ]
        }
    }
}
</script>