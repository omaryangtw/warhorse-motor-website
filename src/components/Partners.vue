<template>
  <div class="bg-black text-gray-100 m-auto px-2 pt-2">
    <div class="container mx-auto">
      <h1 class="text-xl md:text-2xl lg:text-4xl lg:py-6 lg:pl-6 font-semibold">
        Warhorse Partners
      </h1>
      <div class="bg-black flex flex-wrap justify-around text-gray-800">
        <div
          v-for="partner in partners"
          :key="partner"
          class="xl:w-1/6 md:w-3/12 w-4/12 rounded mb-3 m-1 bg-gray-200 bg-opacity-70 transform duration-300 hover:scale-105 hover:bg-opacity-90"
        >
          <a :href="partner.href" target="_blank">
            <img
              :src="partner.url"
              :alt="partner.alt"
              class="border-b border-gray-700"
            />
            <p class="xl:text-lg text-center text-base py-2">
              {{ partner.caption }}
            </p>
          </a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Partners",
  data() {
    return {
      partners: [
        {
          url: require("../../public/partners/startec.webp"),
          alt: "StarTec",
          caption: "Startec Dynamics",
          href: "http://www.startec.com.hk/",
        },
        {
          url: require("../../public/partners/TIK.webp"),
          alt: "TIK",
          caption: "TIK Postons",
          href: "http://www.tik.com.tw/",
        },
        {
          url: require("../../public/partners/YangPo.webp"),
          alt: "YangPo",
          caption: "YangPo Breaks",
          href: "http://yangpo-brakes.com/",
        },
        {
          url: require("../../public/partners/FAR.webp"),
          alt: "FAR",
          caption: "FAR Break System",
          href: "https://www.far-brake.com.tw/",
        },
        {
          url: require("../../public/partners/ANCHOR.webp"),
          alt: "ANCHOR",
          caption: "Anchor Break",
          href: "https://www.anchor-brake.com.tw/",
        },
        {
          url: require("../../public/partners/CCD.webp"),
          alt: "CCD",
          caption: "CCD Factory",
          href: "https://www.facebook.com/CCD-Factory-2148238338754599/",
        },
        {
          url: require("../../public/partners/FEASUN.webp"),
          alt: "FEASUN",
          caption: "FEASUN Technology",
          href: "https://www.feasun3d.com/",
        },
        {
          url: require("../../public/partners/EZECU.webp"),
          alt: "EZECU",
          caption: "EZECU",
          href: "http://www.icleader.com/",
        },
        {
          url: require("../../public/partners/FENGYI.webp"),
          alt: "FENGYI",
          caption: "Feng Yi Steel",
          href: "http://www.fengyi-ti.com/",
        },
        {
          url: require("../../public/partners/Japon.webp"),
          alt: "Japon",
          caption: "Ja-pon Piston Rings",
          href: "https://piston-ring.japon.com.tw/",
        },
        {
          url: require("../../public/partners/KAKUKA.webp"),
          alt: "KAKUKA",
          caption: "KAKUKA Intake System",
          href: "http://www.kakuka.com.tw/",
        },
        {
          url: require("../../public/partners/Hoga.webp"),
          alt: "Hoga",
          caption: "HOGA INDUSTRY",
          href: "http://www.jcmc.com.tw/c-index.htm",
        },
        {
          url: require("../../public/partners/TFM.webp"),
          alt: "TFM",
          caption: "TFM CONTROL CABLE",
          href: "",
        },
        {
          url: require("../../public/partners/HeSeng.webp"),
          alt: "HeSeng",
          caption: "HeSeng",
          href: "",
        },
        {
          url: require("../../public/partners/KMS.webp"),
          alt: "KMS",
          caption: "KMS",
          href: "",
        },
        {
          url: require("../../public/partners/AFS.webp"),
          alt: "AFS",
          caption: "AFS",
          href: "",
        },
      ],
    };
  },
  components: {},
};
</script>

<style></style>
