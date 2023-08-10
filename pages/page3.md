<img class="bg" background-image src='/img/bg.jpg'/>
<br>
<br>
<div> 
  <div class="outbox">
    <div class="column">
      <img src="/img/articles.jpg" style="width:100%;margin:auto">
    </div>
    <div style="width:25%">
      <img src="/img/arrow.png" class = "arrow" >
    </div>
    <div class="column">
      <img v-motion src="/img/Entities.jpg" style="width:80%;margin:auto">
      <p style="text-align: center; font-size: 0.5rem"> names of entities</p>
    </div>
  </div>
</div>
<div class="absolute textbox" style="top:72%;left:10%;right:10%; text-align: justify; width: 800px">
  <span class="textword">
      To support exploration, we analyzed these articles and extracted named entities. These entities are terms and concepts that are familiar to user and serve as topics.
  </span>
</div>

<style>
.textbox .textword{
  background-color: #fff7ed;
  display: inline-block;
  /* line-height: 2; */
  margin: 10px;
  padding: 20px;
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
  .outbox{
    display: flex;
    justify-content: center;
    align-items: center;
  }
  .column {
  float: left;
  width: 90%;
  padding: 1px;
  }
  .arrow{
    margin: auto;
    width:40%;
  }

</style>