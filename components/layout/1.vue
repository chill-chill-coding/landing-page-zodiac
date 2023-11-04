<template>
    <div class="w-auto h-[1775px] px-16 py-28 bg-white flex-col justify-start items-start gap-20 inline-flex">
        <div class="self-stretch h-[156px] flex-col justify-start items-start gap-6 flex">
            <div class="w-[768px] text-neutral-800 text-[40px] font-bold font-['Roboto'] uppercase leading-[48px]">Daily Horoscopes</div>
            <div class="self-stretch text-neutral-800 text-[28px] font-normal font-['Roboto'] leading-[42px]">Tap into the universe’s ancient wisdom with our daily horoscopes, meticulously crafted to guide you through your journey.</div>
        </div>
        <div v-for="(zodiacRow, i) in zodiacsRows" :key="i" class="self-stretch justify-center items-start gap-8 inline-flex">
            <div v-for="zodiac in zodiacRow" :key="zodiac.zodiac"  class="grow shrink basis-0 flex-col justify-start items-start gap-8 inline-flex">
                <img class="self-stretch h-40 rounded-[10px]" :src="`images/zodiacs/${zodiac.image}`" />
                <div class="self-stretch h-[193px] flex-col justify-start items-start gap-6 flex">
                    <div class="self-stretch h-[137px] flex-col justify-start items-center gap-6 flex">
                        <div class="self-stretch h-[65px] flex-col justify-start items-center flex">
                            <div class="self-stretch text-neutral-800 text-2xl font-bold font-['Roboto'] uppercase leading-[33.60px]">{{zodiac.zodiac}}</div>
                            <div class="self-stretch text-neutral-800 text-[22px] font-bold font-['Roboto'] leading-[30.80px]">{{zodiac.date}}</div>
                        </div>
                        <div class="self-stretch text-neutral-800 text-base font-normal font-['Roboto'] leading-normal">{{zodiac.detail}}</div>
                    </div>
                    <button class="self-stretch h-8 pt-2 flex-col justify-start items-start gap-2 flex">
                        <div class="justify-center items-center gap-2 inline-flex">
                            <div class="text-fuchsia-700 text-base font-normal font-['Roboto'] leading-normal">Explore All Horoscopes</div>
                            <div class="w-6 h-6 relative"></div>
                        </div>
                    </button>
                </div>
            </div>
        </div>
    </div>

</template>
<script>
export default {
    data() {
        return {
            zodiacs:[
                {
                    zodiac: "ARIES",
                    date: "March 21 - April 19",
                    detail: "Energetic leaders, passionate and adventurous, with a love for challenges.",
                    image: "image 5.png"
                },
                {
                    zodiac: "TAURUS",
                    date: "April 20 - May 20",
                    detail: "Grounded, enjoys stability and luxury, with a reliable and practical nature.",
                    image: "image 6.png"
                },
                {
                    zodiac: "GEMINI",
                    date: "May 21 - June 20",
                    detail: "Curious and communicative, enjoys variety and is highly adaptable.",
                    image: "image 7.png"
                },
                {
                    zodiac: "CANCER",
                    date: "June 21 - July 22",
                    detail: "Nurturing, emotional, values close relationships, and often protective.",
                    image: "image 8.png"
                },
                {
                    zodiac: "LEO",
                    date: "July 23 - August 22",
                    detail: "Charismatic, loves attention, confident with a flair for drama.",
                    image: "image 9.png"
                },
                {
                    zodiac: "VIRGO",
                    date: "August 23 - September 22",
                    detail: "Detail-oriented, practical, and a perfectionist, with a strong sense of duty.",
                    image: "image 10.png"
                },
                {
                    zodiac: "LIBRA",
                    date: "September 23 - October 22",
                    detail: "Charming, values balance and harmony, seeks justice and fairness.",
                    image: "image 11.png"
                },
                {
                    zodiac: "SCORPIO",
                    date: "October 23 - November 21",
                    detail: "Intense, passionate, mysterious, with a strong will and intuition.",
                    image: "image 12.png"
                },
                {
                    zodiac: "SAGITTARIUS",
                    date: "November 22 - December 21",
                    detail: "Adventurous, optimistic, values freedom and enjoys exploring new ideas.",
                    image: "image 13.png"
                },
                {
                    zodiac: "CAPRICORN",
                    date: "December 22 - January 19",
                    detail: "Ambitious, disciplined, values tradition, and is highly responsible.",
                    image: "image 14.png"
                },
                {
                    zodiac: "AQUARIUS",
                    date: "January 20 - February 18",
                    detail: "Innovative, values independence, humanitarian, and thinks outside the box.",
                    image: "image 15.png"
                },
                {
                    zodiac: "PISCES",
                    date: "February 19 - March 20",
                    detail: "Compassionate, artistic, dreamy, with a deep sense of empathy.",
                    image: "image 16.png"
                },
            ]
        }
    },
    computed: {
        zodiacsRows () {
            return this.zodiacs.reduce((acc, n, i) => {
                i % 4 ? acc[acc.length - 1].push(n) : acc.push([n])
                return acc
            },[])
        }
    }
}
</script>
<style lang="">
    
</style>