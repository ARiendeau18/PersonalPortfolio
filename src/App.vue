<!-- Andrew Riendeau -->
<script>



export default({
      el: '#mainId',
      data(){
        return {
        
          isShow: true,
          isShow2: true,
          num: null,
        
        }

      },
      methods: {
        three() {
          this.num = 3;
        },
        two() {
          this.num = 2;
        },
        four() {
          this.num = 4;
        },
        five() {
          this.num = 5;
        },
      }
    }) 


    

</script>

 

<template>
<div class="whole" style="width 100%; height: 600px;">
  <header>
    <br>
    <button @click="two" class="num" style="margin-right: 10px;">Resume</button>
    <button @click="three" class="num" style="margin-right: 10px;">Projects</button>
    <button @click="four" class="num" style="margin-right: 10px;">Course Work</button>
    <button @click="five" class="num" >Contact Information</button>
  </header>
  <br>
  <div class="imgBack" style="width: 25%; float: left; height: 100%;" >
  <img src="./assets/IMG_1040.png">
  </div>
  <div class="textBack" style="width: 75%; float: left; height: 100%;">
      <div class="temp" v-show="num == null">
        My Name is Andrew Riendeau and I am a senior at 
        the University of North Carolina at Charlotte. I have had a passion for computer science since I began coding in highschool. 
        At UNCC, I majored in Computer Science with a concentration in Cyber Security and I have a minor in Mathematics. 
      </div>
      <div class="temp" style="display:none;" v-show="num == 2">
        <img src="./assets/res1pic.png" style="width: 553px; height: 718px;"/>
      </div>

      <div class="temp" style="display:none;" v-show="num == 3">
        Machine Learning Program that Models and Predicts solar power generation based on the weather with a near 70% accuracy.
        <img src="./assets/ML.png" style="width: 553px; height: 500px;"/>
        Technical Projects:
        <img src="./assets/TechPro.png" style="width: 525px; height: 250px;"/>
      </div>

      <div class="temp" style="display:none;" v-show="num == 4">
        Selected Coursework: Data Structures and Algorithms, Computer Forensics, Database Design and Implementation, 
        IT Infrastructure and Security, Network Based Application Development, Security Analytics, Secure Programming and 
        Penetration Testing
      </div>

      <div class="temp" style="display:none;" v-show="num == 5">
        email: riendeauandrew@gmail.com <br>
        cell: 980-245-0507
      </div>

    

    </div>
</div>


</template>

<style>
@import './assets/base.css';

#app {
  max-width: 1280px;
  margin: 0 auto;
  padding: 2rem;

  font-weight: normal;
  
}

img {
  padding: 5%;
  width: 100%;
  height: 100%;
}


p {
  width: 20%;
  color: aliceblue;
}

.whole{
  border: 5px, solid, blueviolet;
  margin: auto;
  text-align: center;
  
}

.imgBack {
  background-color: rgb(15, 20, 20);
  border: 5px, blueviolet;
  
}
.textBack {
  background-color: rgb(15, 20, 20);
  text-align: center;
  padding: 100px;
  border: 5px, blueviolet;
  
  
}
.temp{
  background-color: rgb(255, 255, 255);
  width: 100%;
  height: 100%;
  text-align: center;
  padding: 100px;
  font-size: medium;
  color: rgb(0, 0, 0);
  border-style: solid;
  border: 5px, solid, blueviolet;
  overflow: auto;
  
  border-width: 100%;
  
}

.whole {
  background-color:blueviolet;
}

button {
  height: 30px;
  width: 170px;
  
}


</style>

