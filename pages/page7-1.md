<img class="bg" background-image src='/img/bg.jpg'/>
<br>
<div>
    <div class="container" style="display: flex; justify-content: center">
        <img src="/img/scatterplot.jpg" class="h-65"  />
    </div>
    <div >
        <img src="/img/square.png" class=" motion absolute h-32 top-5rem right-21.3rem ">
        <p class="motion text absolute top-6.5rem right-6rem w-50 h-50">Mixed topics has high volume of articles, which means that these topics are more controvertial. Thus, media outlets are more likely to have bias on these topics. <span style="font-weight: 600">We encourage user to explore topics located in this area.</span></p>
    </div>
</div>
<div class="absolute textbox" style="text-align: justify;top:60%;left:10%;right:10%;"> 
    <span class="textword">
        After understanding how we encode our data, let's explain visualization we have created on NOVA.
        <span >
            We visualize a scatter plot and categorize the topics into four types: <span class="neg_color">negative</span>, <span class="mix_color">mixed</span>, <span class="neu_color">neutral</span>, and <span class="pos_color">positive</span> with threshold 0.5 on both x and y axis for default. User can adjust the threshold by dragging the segmentation <span class="last_word"> point <svg width="20" height="20"> <rect x=5 y=9 width=10 height=10 fill="white" stroke="black" stroke-width="1"/> </svg> </span>base on their personal believe.
        </span>
    </span>

</div>


<style>
.textbox{
  background-color: #fff7ed;
  /* border-radius: 1.5rem; */
  color: #000;
  display: inline;
}
.textbox .textword{
  background-color: #fff7ed;
  display: inline-block;
  /* line-height: 2; */
  margin: 10px;
  padding: 20px;
}
    .bg{
    opacity:0.1;
    position:absolute;
    left:0;
    top:0;
    width:100%;
    height:auto;
}
    .last_word {
    /* Stick icon to last word */
    white-space: no-wrap;  
    
    /* Make sure last word and icon will break ultimately */
    display: inline-flex;
    flex-wrap: wrap; 
}
  .motion{
    animation: clickit 5s;
  }
    @keyframes clickit {
        0% {opacity: 0}
        80% {opacity: 0}
        100% {opacity: 1}
  }
  .text{
    font-size: 10px;
    text-align: justify;
    /* background-color:#fff; */
  }
    .neg_color{
    background-color: #f4c49c;
    opacity:1.0;
  }
  .pos_color {
    background: #baf0f5;
}
  .neu_color {
    background: #dddddd;
  }
  .mix_color{
    background-image: linear-gradient(-45deg, #f4c49c 25%, #baf0f5 25%, #baf0f5 50%, #f4c49c 50%, #f4c49c 75%, #baf0f5 75%, #baf0f5 100%);
    background-size: 20px 20px;
}
</style>