<template>
<section class="features">
  <div class="features-center">
  <div class="features-toggle">0</div>
  <div class="features-circles_container">
    <div class="features-circle">X</div>
    <div class="features-circle">X</div>
    <div class="features-circle">X</div>
    <div class="features-circle">X</div>
    <div class="features-circle">X</div>
    <div class="features-circle">X</div>
    <div class="features-circle">X</div>
    <div class="features-circle">X</div>
  </div>
  </div>
</section>
</template>

<script>
export default {
  name: "FeaturesSection"
}
</script>

<style lang="scss" scoped>
  .features{
    height: 100vh;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;

    .features-center{
        position: relative;
        border: 1px solid black;

      .features-toggle{
        position: absolute;
      }

      .features-circles_container{
        position: relative;
        width: 100px;
        height: 100px;
        border: 1px solid black;
        
        .features-circle{
          position: absolute;
        }

        .features-circle:nth-child(1){
          left: 0;
        }

        .features-circle:nth-child(2){
          left: 50%;
          transform: translateX(-50%);
        }

        .features-circle:nth-child(3){
            right: 0;
        }

        .features-circle:nth-child(4){
            top: 50%;
            transform: translateY(-50%);
        }

        .features-circle:nth-child(5){
          top: 50%;
          right: 0;
          transform: translateY(-50%);
        }

        .features-circle:nth-child(6){
          bottom: 0;
        }

        .features-circle:nth-child(7){
          bottom: 0;
          left: 50%;
          transform: translateX(-50%);
        }

        .features-circle:nth-child(8){
          bottom: 0;
          right: 0;
        }

      }
    }
  }
</style>