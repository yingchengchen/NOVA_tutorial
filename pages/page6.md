<img class="bg" background-image src='/img/bg.jpg'/>
<br>
<br>
<br>
<div>
  <div class="outbox">
    <div class="column">
        <img src="/img/articles_withSenti.jpg" style="width:100%">
    </div>
    <div style="width:25%">
        <img src="/img/arrow.png" class = "arrow" >
        <br>
    </div>
    <div class="column">
        <img src="/img/Topics3.jpg" style="margin:auto;width:90%">
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
        <img src="/img/6.jpg" style="width:95%;margin:auto">
    </div>
  </div>
</div>
<div class="absolute textbox" style="text-align: justify;top:55%;left:10%;right:10%;"> 
  <span class="textword">
    In addition to encoding the interest a topic received from media outlets, we also encode the sentiment type of each topic derived from the content of related articles.<span >
    We count both the number of negative and positive articles per topic. Then we use min-max normalization on both counts and assign (<span class="pos_color">score<sub>pos</sub></span>, <span class="neg_color">score<sub>neg</sub></span>). This value is used to determone the position of each dot. We plot each topic using score<sub>pos</sub> as x-coordinate and score<sub>neg</sub> as y-coordinate on the 2-D scatter plot.</span>
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
