<template>
    <div class="w-full h-11/12 px-16 py-28 bg-white flex-col justify-center items-center gap-20 inline-flex">
        <div class="h-[136px] flex-col justify-start items-center gap-4 flex">
            <div class="self-stretch h-[136px] flex-col justify-start items-center gap-6 flex">
                <div class="self-stretch text-center text-neutral-800 text-5xl font-bold font-['Roboto'] leading-[57.60px]">Zodiac Accessories</div>
                <div class="self-stretch text-center text-neutral-800 text-lg font-normal font-['Roboto'] leading-[27px]">Explore our curated collection of mystical treasures, zodiac-inspired accessories, and spiritual tools.</div>
            </div>
        </div>
        <div class="self-stretch justify-center items-start gap-8 grid grid-cols-4 gap-y-20">
            <div v-for="accessory in accessories" class="grow shrink basis-0 flex-col justify-start items-start gap-8 inline-flex">
                <LayoutCard3 :accessory="accessory"/>
            </div>
        </div>
        <button class="flex-col justify-start items-center gap-16 flex">
            <div class="px-6 py-3 border border-fuchsia-700 justify-center items-center gap-2 inline-flex">
                <div class="text-fuchsia-700 text-base font-normal font-['Roboto'] leading-normal">View all</div>
            </div>
        </button>
    </div>
</template>
<script>
export default {
    data() {
        return {
            accessories: [
                {
                    header: "Aries Zodiac Charm Bracelet",
                    price: 29.99,
                    detail: "Vibrant red beads with an Aries ram charm; infuses confidence and courage for daily challenges.",
                    image: "image 23.png"
                },
                {
                    header: "Taurus Zodiac Scented Candle",
                    price: 24.99,
                    detail: "Earthy and calming scents to relax and ground Taurus energy; adorned with Taurus symbols.",
                    image: "image 24.png"
                },
                {
                    header: "Gemini Zodiac Phone Case",
                    price: 19.99,
                    detail: "Sleek, protective case featuring a Gemini twin design; perfect for the communicative and lively Gemini.",
                    image: "image 25.png"
                },
                {
                    header: "Moonlit Crab Cancer Zodiac Ring",
                    price: 45.99,
                    detail: "Elegant silver ring featuring a delicate crab design, embodying Cancer's nurturing spirit and connection to the moon.",
                    image: "image 26.png"
                },
                {
                    header: "Regal Mane Leo Zodiac Wallet",
                    price: 59.99,
                    detail: "Luxurious leather wallet embossed with a majestic lion, capturing Leo’s bold spirit and love for the finer things.",
                    image: "image 27.png"
                },
                {
                    header: "Virgo Zodiac Planner",
                    price: 22.99,
                    detail: "Organize life meticulously with this Virgo-themed planner; includes zodiac-specific advice and goal-setting sections.",
                    image: "image 28.png"
                },
                {
                    header: "Harmonic Scales Libra Music Box",
                    price: 74.99,
                    detail: "Exquisite music box featuring balanced scales, playing a harmonious melody to soothe and delight any Libra’s heart.",
                    image: "image 29.png"
                },
                {
                    header: "Scorpio Zodiac Mystery Box",
                    price: 39.99,
                    detail: "A surprise assortment of Scorpio-themed accessories; perfect for the enigmatic and passionate Scorpio.",
                    image: "image 30.png"
                },
                {
                    header: "Sagittarius Celestial Archer Bookmark",
                    price: 14.99,
                    detail: "Sleek, metallic bookmark with an intricately designed arrow, perfect for the adventurous Sagittarius who loves to read.",
                    image: "image 31.png"
                },
                {
                    header: "Capricorn Steadfast Summit Keychain",
                    price: 12.99,
                    detail: "Durable keychain featuring a detailed mountain goat, a daily reminder of Capricorn’s resilience and ambition.",
                    image: "image 32.png"
                },
                {
                    header: "Aquarian Essence Diffuser",
                    price: 49.99,
                    detail: "Innovative diffuser design inspired by the Water Bearer, spreading calming scents and Aquarius’ humanitarian vibes.",
                    image: "image 33.png"
                },
                {
                    header: "Celestial Pisces Canvas Art",
                    price: 29.00,
                    detail: "Beautiful dream catcher featuring two fish swimming in a circle, capturing the imaginative and empathetic spirit of Pisces.",
                    image: "image 34.png"
                },
            ]
        }
    }
}
</script>
<style lang="">
    
</style>