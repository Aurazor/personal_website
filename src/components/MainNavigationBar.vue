<template>
  <nav>
    <a href="#"><img src="../assets/logo.png"  class="logo"></a>
    <div class="toggle"></div>
    <ul class="navigation">
      <li><a href="#">Home</a></li>
      <li><a href="#">Menu</a></li>
      <li><a href="#">What's new</a></li>
      <li><a href="#">Contact</a></li>
    </ul>
  </nav>
</template>

<script>
export default {
  name: "MainNavigationBar"
}
</script>

<style lang="scss" scoped>
  nav{
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    padding: 20px 100px;
    display: flex;
    justify-content: space-between;
    align-items: center;

      .logo{
        position: relative;
        max-width: 80px;
      }

      ul{
        position: relative;
        display: flex;

        li{
          list-style: none;

          a{
            display: inline-block;
            color: #333;
            font-weight: 400;
            margin-left: 40px;
            text-decoration: none;
          }
        }
      }
  }


</style>