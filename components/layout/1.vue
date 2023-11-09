<template>
  <div
    class="w-full h-11/12 px-16 py-28 bg-white flex-col justify-start items-start gap-20 inline-flex">
    <div
      class="self-stretch h-1/6 flex-col justify-start items-start gap-6 flex">
      <div
        class="w-1/3 text-neutral-800 text-[40px] font-bold font-['Roboto'] uppercase leading-[48px]">
        Daily Horoscopes
      </div>
      <div
        class="self-stretch text-neutral-800 text-[28px] font-normal font-['Roboto'] leading-[42px]">
        Tap into the universe’s ancient wisdom with our daily horoscopes,
        meticulously crafted to guide you through your journey.
      </div>
    </div>
    <div
      class="self-stretch justify-center items-start gap-8 grid grid-cols-4 gap-y-20">
      <div
        v-for="zodiac in zodiacs"
        :key="zodiac.zodiac"
        class="grow shrink basis-0 flex-col justify-start items-start gap-8 inline-flex">
        <LayoutCard1 :zodiac="zodiac" />
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      zodiacs: [
        {
          title: "ARIES",
          date: "March 21 - April 19",
          detail:
            "Energetic leaders, passionate and adventurous, with a love for challenges.",
          image: "image 5.png",
        },
        {
          title: "TAURUS",
          date: "April 20 - May 20",
          detail:
            "Grounded, enjoys stability and luxury, with a reliable and practical nature.",
          image: "image 6.png",
        },
        {
          title: "GEMINI",
          date: "May 21 - June 20",
          detail:
            "Curious and communicative, enjoys variety and is highly adaptable.",
          image: "image 7.png",
        },
        {
          title: "CANCER",
          date: "June 21 - July 22",
          detail:
            "Nurturing, emotional, values close relationships, and often protective.",
          image: "image 8.png",
        },
        {
          title: "LEO",
          date: "July 23 - August 22",
          detail:
            "Charismatic, loves attention, confident with a flair for drama.",
          image: "image 9.png",
        },
        {
          title: "VIRGO",
          date: "August 23 - September 22",
          detail:
            "Detail-oriented, practical, and a perfectionist, with a strong sense of duty.",
          image: "image 10.png",
        },
        {
          title: "LIBRA",
          date: "September 23 - October 22",
          detail:
            "Charming, values balance and harmony, seeks justice and fairness.",
          image: "image 11.png",
        },
        {
          title: "SCORPIO",
          date: "October 23 - November 21",
          detail:
            "Intense, passionate, mysterious, with a strong will and intuition.",
          image: "image 12.png",
        },
        {
          title: "SAGITTARIUS",
          date: "November 22 - December 21",
          detail:
            "Adventurous, optimistic, values freedom and enjoys exploring new ideas.",
          image: "image 13.png",
        },
        {
          title: "CAPRICORN",
          date: "December 22 - January 19",
          detail:
            "Ambitious, disciplined, values tradition, and is highly responsible.",
          image: "image 14.png",
        },
        {
          title: "AQUARIUS",
          date: "January 20 - February 18",
          detail:
            "Innovative, values independence, humanitarian, and thinks outside the box.",
          image: "image 15.png",
        },
        {
          title: "PISCES",
          date: "February 19 - March 20",
          detail:
            "Compassionate, artistic, dreamy, with a deep sense of empathy.",
          image: "image 16.png",
        },
      ],
    };
  }
};
</script>
<style lang=""></style>
