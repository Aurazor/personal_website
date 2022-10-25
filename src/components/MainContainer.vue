<template>
  <div class="container">
    <MainSection/>
    <FeaturesSection/>
    <TimelineSection/>
  </div>
</template>

<script>
import MainSection from "@/components/MainSection";
import FeaturesSection from "@/components/FeaturesSection";
import TimelineSection from "@/components/TimelineSection";
export default {
  name: "MainContainer",
  components:{
    MainSection,
    FeaturesSection,
    TimelineSection
  }

}
</script>

<style lang="scss">
  .container{
    margin: 0 auto;
  }
</style>