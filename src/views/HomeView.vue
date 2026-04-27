<template>
  <main>
    <MyPortfolio />
    <MySkills />
    <MyWorks />
    <ContactUs />
  </main>
</template>

<script>
import MyPortfolio from "@/components/MyPortfolio.vue";
import MySkills from "@/components/MySkills.vue";
import MyWorks from "@/components/My-Works.vue";
import ContactUs from "@/components/ContactUs.vue";
export default {
  components: {
    MyPortfolio,
    MySkills,
    MyWorks,
    ContactUs,
  },
};
</script>
