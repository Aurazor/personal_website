<template>
  <section class="timeline">
    <div class="timeline-wrapper">
      <div class="timeline-header">
          <h1>Qualification</h1>
          <span>My Personal Journey</span>
      </div>
      <div class="timeline-container">
        <div class="timeline-container_header">
          <div class="active-timeline"><ion-icon name="school-outline"></ion-icon>Education</div>
          <div><ion-icon name="briefcase-outline"></ion-icon>Work</div>
        </div>
        <div class="timeline-container_history">

           <div class="timeline-box">
             <div class="timeline-box_text">


             <div class="timeline-box_title">
               Computer Engineer
             </div>
             <div class="timeline-box_location">
               Peru - University
             </div>
             <div class="timeline-box_date">
               <ion-icon name="calendar-outline"></ion-icon>2019 - 2014
             </div>
             </div>
           </div>

          <div class="timeline-box">
            <div class="timeline-box_text">

            <div class="timeline-box_title">
              Computer Engineer
            </div>
            <div class="timeline-box_location">
              Peru - University
            </div>
            <div class="timeline-box_date">
              <ion-icon name="calendar-outline"></ion-icon>2019 - 2014
            </div>
              </div>
          </div>

          <div class="timeline-box">
            <div class="timeline-box_text">

            <div class="timeline-box_title">
              Computer Engineer
            </div>
            <div class="timeline-box_location">
              Peru - University
            </div>
            <div class="timeline-box_date">
              <ion-icon name="calendar-outline"></ion-icon> 2019 - 2014
            </div>
              </div>
          </div>

          <div class="timeline-box">
            <div class="timeline-box_text">

              <div class="timeline-box_title">
                Computer Engineer
              </div>
              <div class="timeline-box_location">
                Peru - University
              </div>
              <div class="timeline-box_date">
                <ion-icon name="calendar-outline"></ion-icon> 2019 - 2014
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "TimelineSection"
}
</script>

<style lang="scss" scoped>
@import "src/assets/_helpers/_variables.scss";

  .timeline{
    height: 100vh;

    ion-icon{
      margin-right: 5px;
    }


    .timeline-wrapper{
      display: flex;
      flex-direction: column;
      justify-content: space-evenly;
      align-items: center;
      height: 100%;

      .timeline-container{
        width: 400px;
        //border: 1px solid black;
        position: relative;
        .timeline-container_header{
          display: flex;
          justify-content: space-evenly;
          margin-bottom: 50px;

          .active-timeline{
            color: $color-primary;
          }

          div{
            display: flex;
            justify-content: center;
            align-items: center;
          }

        }

        .timeline-container_history{

          //line
          &:before{
            content: "";
            position: absolute;
            left: 50%;
            width: 3px;
            height: 63%;
            background: black;
            display: block;
          }

          .timeline-box{
            position: relative;
            //border: 1px solid black;
            width: 50%;


            //timeline-box round-indicator
            &:before{
              content: '';
              position: absolute;
              width: 10px;
              height: 10px;
              border-radius:20px ;
              //transform: translate(-50%, -50%);
              background: $color-primary;
            }

            &:nth-child(odd){
              &:before{
                right: 0;
                transform: translate(60%);
              }
            }

            &:nth-child(even){
              left: 50%;

              display: flex;
              justify-content: flex-end;
              align-items: center;

              &:before{
                top: 0;
                left: 0;
                transform:translateX(-40%);
              }
            }

            .timeline-box_text{
              width: 90%;
              border-radius: 5px;
              background-color: $color-gray;
              padding: 10px;
              text-align: center;

              .timeline-box_title{
                font-weight: bold;
              }

              .timeline-box_location{
                font-size: 15px;
              }

              .timeline-box_date{
                font-weight: 300;
                font-size: 12px;
                display: flex;
                justify-content: center;
                align-items: center;
              }
            }
          }
        }
      }
    }

  }
</style>