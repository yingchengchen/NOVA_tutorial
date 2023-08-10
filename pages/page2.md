<img class="bg" background-image src='/img/bg.jpg'/>
<h1>How does <span style="font-style: italic">NOVA</span> work? </h1>
<div>
  <br><br>
  <img
      v-motion
      :initial="{ x: 100,y:500}"
      :enter="final_NY"
      class="absolute h-27"
      src="/img/New York Times_articles.png"
  />
  <img
      v-motion
      :initial="{ x: 320,y:500}"
      :enter="final_CNN"
      class="absolute h-18"
      src="/img/CNN_articles.png"
  />
  <img
      v-motion
      :initial="{ x: 150,y:0}"
      :enter="final_FOX"
      class="absolute h-22"
      src="/img/FoxNews_articles.png"
  />
  <img
      v-motion
      :initial="{ x: 350,y:-80}"
      :enter="final_B"
      class="absolute h-27"
      src="/img/Breitbart_articles.png"
  />
  <img
      v-motion
      :initial="{ x: 500,y:0}"
      :enter="final_WP"
      class="absolute h-27"
      src="/img/Washington Post_articles.png"
  />
  <img
      v-motion
      :initial="{ x: 500,y:500}"
      :enter="final_ABC"
      class="absolute h-25"
      src="/img/ABC News_articles.png"
  />  
</div>
<div class="absolute textbox circle " style="top:64%;left:10%;right:10%; text-align: justify; width: 800px" >
  <span class="textword">
      <span style="font-style: italic">NOVA</span> offers a means to explore an individual's potential <span style="font-style:italic"> echo chamber </span> when it comes to online mainstream media outlets. Each news oulet has its own coverage and possible biases. Typically the average person receives their news from a subset of these outlets they trust. <span style="font-style: italic">NOVA</span> enables users to explore outside of their own universe and assess their assumptions of other outlets.
  </span>
</div>
<img class="circle absolute h-30 right-17.8rem top-11rem" src="/img/circle.png"/>
<script setup lang="ts">
const final_NY = {
  x:250,
  y:80,
  transition: {
    type: 'spring',
    damping: 10,
    stiffness: 20,
    mass: 2
  }
}
const final_CNN = {
  x:340,
  y:50,
  transition: {
    type: 'spring',
    damping: 10,
    stiffness: 20,
    mass: 2
  }
}
const final_FOX = {
  x:250,
  y:-20,
  transition: {
    type: 'spring',
    damping: 10,
    stiffness: 20,
    mass: 2
  }
}
const final_B = {
  x:355,
  y:-60,
  transition: {
    type: 'spring',
    damping: 10,
    stiffness: 20,
    mass: 2
  }
}
const final_WP = {
  x:450,
  y:-40,
  transition: {
    type: 'spring',
    damping: 10,
    stiffness: 20,
    mass: 2
  }
}
const final_ABC = {
  x:450,
  y:90,
  transition: {
    type: 'spring',
    damping: 10,
    stiffness: 20,
    mass: 2
  }
}
</script>

<style>
.slidev-layout h1{
 color: black;
 /* margin-top: 3rem; */
 margin-bottom: 1rem;
 margin-left: 0rem;
}
.textbox .textword{
  background-color: #fff7ed;
  display: inline-block;
  /* line-height: 2; */
  margin: 10px;
  padding: 18px;
}
.textbox{
  background-color: #fff7ed;
  /* border-radius: 1.5rem; */
  color: #000;
  display: inline;
}
.bg{
  opacity:0.1;
  position:absolute;
  left:0;
  top:0;
  width:100%;
  height:auto;
}
  .center{
  /* width: 60%; */
  margin: auto;
  display: block;
}
  .circle{
    animation: clickit 1.9s
  }
    @keyframes clickit {
        0% {opacity: 0}
        80% {opacity: 0}
        100% {opacity: 1}
    }
</style>
