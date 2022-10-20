<template>
 <section class="main-section">
   <div class="circle"></div>
   <MainNavigationBar/>
   <div class="content">
     <div class="textBox">
       <h2>Hello World<br>I'm <span>Nikhil Aukhaj</span></h2>
       <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Porro officiis totam aliquam recusandae distinctio illum ducimus? Aperiam dolor autem quis nemo, vero esse nam optio cumque ratione reiciendis a temporibus!</p>
       <a href="#">Learn More</a>
     </div>
     <div class="imgBox">
       <img src="../assets/images/kush.png" class="starbucks">
     </div>
   </div>
<!--   <ul class="thumb">-->
<!--     <li><img src="../assets/images/thumb1.png" onclick="imgSlider('images/img1.png');changeCircleColor('#017143')" alt=""></li>-->
<!--     <li><img src="../assets/images/thumb2.png" onclick="imgSlider('images/img2.png');changeCircleColor('#eb7495')" alt=""></li>-->
<!--     <li><img src="../assets/images/thumb3.png" onclick="imgSlider('images/img3.png');changeCircleColor('#d752b1')" alt=""></li>-->
<!--   </ul>-->
   <div class="sci">
     <li><a href="#"><img src="../assets/images/facebook.png" alt=""></a></li>
     <li><a href="#"><img src="../assets/images/twitter.png" alt=""></a></li>
     <li><a href="#"><img src="../assets/images/instagram.png" alt=""></a></li>
   </div>
 </section>
</template>

<script>
import MainNavigationBar from "@/components/MainNavigationBar";
export default {
  name: "MainSection",
  components:{
    MainNavigationBar
  }
}
</script>

<style lang="scss" scoped>
  .main-section{
    position:relative;
    width: 100%;
    height: 100vh;
    padding:100px;
    display:flex;
    justify-content: space-between;
    align-items: center;
    background: #fff;

    .content{
      //position: relative;
      width: 100%;
      display: flex;
      justify-content: space-between;
      align-items: center;

      .textBox{
        position: relative;
        max-width: 600px;

        h2{
          color: #333;
          font-size: 4em;
          line-height: 1.4em;
          font-weight: 500;

          span{
            color: #017143;
            font-size: 1.2em;
            font-weight: 900;
          }
        }

        a{
          display: inline-block;
          margin-top: 20px;
          padding: 8px 20px;
          background: #017143;
          color: #fff;
          border-radius: 40px;
          font-weight: 500;
          letter-spacing: 1px;
          text-decoration: none;
        }
      }

      .imgBox{
        width: 600px;
        display: flex;
        justify-content: center;
        padding-right: 50px;
        margin-top: 50px;

        img{
          position: absolute;
          bottom: 0;
          max-width: 340px;
        }
      }
    }

    .thumb{
      position: absolute;
      left: 50%;
      bottom: 20px;
      transform:translate(-50%);
      display: flex;

      li{
        list-style: none;
        display: inline-block;
        margin: 0 20px;
        cursor: pointer;
        transition: 0.5s;

        &:hover{
          transform:translateY(-15px) ;
        }

        img{
          max-width: 60px;
        }
      }
    }

    .sci{
      position: absolute;
      top: 50%;
      right: 30px;
      transform: translateY(-50%);
      display: flex;
      justify-content: center;
      align-items: center;
      flex-direction: column;

      li{
        list-style: none;

        a{
          display: inline-block;
          margin: 5px 0;
          transform:scale(0.6);
          filter: invert(1);
        }
      }
    }

    .circle{
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: #017143;
      clip-path: circle(600px at right 800px);
    }
  }
</style>