<script>
import TheFifthSection from "./TheFifthSection.vue";
import TheFirstSection from "./TheFirstSection.vue";
import TheFourthSection from "./TheFourthSection.vue";
import TheSecondSection from "./TheSecondSection.vue";
import TheThirdSection from "./TheThirdSection.vue";
export default {
  components: {
    TheFirstSection,
    TheSecondSection,
    TheThirdSection,
    TheFourthSection,
    TheFifthSection,
  },
  data() {
    return {};
  },
  methods: {},
  mounted() {},
};
</script>

<template>
  <TheFirstSection></TheFirstSection>
  <TheSecondSection></TheSecondSection>
  <TheThirdSection></TheThirdSection>
  <TheFourthSection></TheFourthSection>
  <TheFifthSection></TheFifthSection>
</template>

<style lang="scss" scoped></style>
