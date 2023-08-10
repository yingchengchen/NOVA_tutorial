<img class="bg" background-image src='/img/bg.jpg'/>
<br>
<br>
<br>
<div>
  <div class="outbox">
    <div class="column">
        <img src="/img/articles_withTopics.jpg" style="width:100%">
    </div>
    <div style="width:25%">
        <img src="/img/arrow.png" class = "arrow" >
        <br>
    </div>
    <div class="column">
        <img src="/img/Topics1.jpg" style="margin:auto;width:75%">
    </div>
    <div style="width:25%">
        <img src="/img/arrow.png" class = "arrow" >
        <div class="box" style="width:100%;margin:auto">
            <span class="encode" style="font-style: italic">
                    data encoding
            </span>
        </div>
    </div>
    <div class="column">
        <img src="/img/dots_5.jpg" style="width:70%;margin:auto;">
    </div>
  </div>
</div> 
<div class="absolute textbox" style="text-align: justify;top:55%;left:10%;right:10%;"> 
  <span class="textword">
      However, a dot doesn't reveal that much information. Not all topics received equal attention and had same number of articles written about them. 
      <span>We count the total number of articles related to the same topic and using a linear scale color encode each dot. A deepper purple hue implies more articles were written related to that topic. As we see above, there are 1557 articles related to <span style="font-weight: 600;font-style: italic">Donald Trump</span> and there are 87 articles for <span style="font-weight: 600;font-style: italic">The Times</span>. Therefore, the purple dot for <span style="font-weight: 600;font-style: italic">Donald Trump</span> is much darker than the dot for <span style="font-weight: 600;font-style: italic">The Times</span>.</span>
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
  width: 80%;
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
