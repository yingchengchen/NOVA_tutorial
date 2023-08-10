<img class="bg" background-image src='/img/bg.jpg'/>
<br>
<div> 
  <div class="outbox ">
    <div class="column">
      <img src="/img/scatterplot1.jpg" style="width:100%;">
    </div>
    <div style="width:20%;">
      <img src="/img/arrow.png" class = "arrow" >
        <div class="box" style="width:45%;margin:auto">
            <span class="encode" style="font-style: italic">
                    data encoding
            </span>
        </div>
    </div>
    <div class="column">
      <img src="/img/scatterplot2.jpg" style="width:100%;">
    </div>
  </div>
</div>
<div class="absolute textbox" style=" text-align: justify;top:60%;left:10%;right:10%;">
  <span class="textword">
      Although user can reset the segmentation rule, here are some limitations on the adjustment, since the sentiment score on each topic is fixed. For example, we cannot categorize <span style="font-weight: 600;font-style: italic">China</span> as negative and <span style="font-weight: 600;font-style: italic">White_House</span> as mixed at the same time, this is because the article of <span style="font-weight: 600;font-style: italic">China</span> is more polarized than that of <span style="font-weight: 600;font-style: italic">White_House</span>. <span style="font-weight: 600"> But the opposite is possible.</span>
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
  .outbox{
    display: flex;
    justify-content: center;
    align-items: center;
  }
  .column {
  float: left;
  width: 37%;
  padding: 1px;
  }
  .arrow{
    margin: auto;
    width:25%;
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
