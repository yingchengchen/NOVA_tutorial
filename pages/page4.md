<img class="bg" background-image src='/img/bg.jpg'/>
<br>
<br>
<div> 
  <div class="outbox">
    <div style="column">
        <img src="/img/EntitiesLink.jpg" style="width:90%">
    </div>
    <div style="width:25%">
        <img src="/img/arrow.png" class = "arrow" >
        <div class="box" style="width:70%;margin:auto">
            <span class="encode" style="font-style: italic">
                    data encoding
            </span>
        </div>
    </div>
    <div style="width: 60%;">
        <img src="/img/dots_4.jpg" style="width:70%" class="ml-3rem">
    </div>
  </div>
</div>
<div class="absolute textbox" style="text-align: justify;top:65%;left:10%;right:10%;"> 
  <span class="textword">
      Entites may have many forms, for example, <span style="font-style: italic">Donald Trump</span>, <span style="font-style: italic">Trump</span> and <span style="font-style: italic">President Trump</span>, that are associated with a single topic,  <span style="font-weight: 600;font-style: italic">Donald Trump</span>. We link entities mentioned in different articles by Wikipedia ID and generate as a single topic. We visually encode each topic as a dot.
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
    .box{
        /* background-color: #3c3f41; */
        width: max-content;
        display: flex;
    }
    .encode{
        font-size: 13px;
        color: #000;
        overflow: hidden;
        white-space: nowrap;
        margin: 0 auto;
        animation:
            typing 1s steps(20),
            cursor 0.5s;
    }
    @keyframes typing {
        from{ width: 0 }
        to{ width: 100% }
    }
</style>
