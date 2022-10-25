<template>

  <MainContainer/>
  <div>
    <component :is="'script'" type="module" src="https://unpkg.com/ionicons@5.5.2/dist/ionicons/ionicons.esm.js"></component>
    <component :is="'script'" nomodule src="https://unpkg.com/ionicons@5.5.2/dist/ionicons/ionicons.js"></component>
  </div>
</template>

<script>
import MainContainer from "@/components/MainContainer";
export default {
  name: 'App',
  components: {
    MainContainer
  }
}


</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@100;300;400;500&display=swap');
@import "src/assets/_helpers/_custom_styles.scss";

body{
  font-family: 'Poppins', sans-serif;

}


</style>
