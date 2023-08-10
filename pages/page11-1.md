<img class="bg" background-image src='/img/bg.jpg'/>
<br>
<br>
<div style="height:400px"> 
    <div class="box">
        Steps we suggest for user to do in <span font-style: italic>Inspection </span> page: 
        <img src="/img/Inspection.jpg" class="h-15" style="float:right">
    </div>
    <div class="container">
        <ol class="list">
            <li>Investigate and observe both negative and positive articles of the topics. Do you find any entity is misclassified as a wrong topic? Are there any bias in terms of word choice or unverified stories in the articles?</li>
            <li>Write down your thought and your findings. Do you think the outlet has bias, or do you agree with their points of view?</li>
            <li>After reviewing the content, do you change your perspective to the outlet? Think about which outlet you would choose the next time you want to know the news information! </li>
        </ol>
    </div>
</div>
<div style="width:600px">
  <div style="float:right">
    <div class="text absolute" style="font-style: italic">
        Try out our system by youself <carbon:arrow-right class="inline"/>
      <img src="/img/nova_logo.png" class="h-5 pb-3px cursor-pointer zoom" 
      style="float:right"
      @click="$slidev.nav.next"
      >
    </div>
  </div>
</div>


<style>
.bg{
  opacity:0.1;
  position:absolute;
  left:0;
  top:0;
  width:100%;
  height:auto;
}
.box{
    width:750px;
} 
.text{
  width:220px;
  bottom: 4rem;
  font-size: 0.8rem;
}
.zoom{
  transition: transform .2s;
}
.zoom:hover{
  transform: scale(1.5);
}
ol li:not(:last-child) {
  margin-bottom: 20px;
}
        
ol {
  /* max-width: 350px; */
  counter-reset: counter;
  list-style: none;
  padding-left: 40px;
}
ol li {
  list-style-type: none;
  margin: 0 0 0.5rem 0;
  counter-increment: counter;
  position: relative;
}
ol li::before {
  content: counter(counter);
  color: #155e75;
  background-color: #f9dd94;
  font-size: 1rem;
  font-weight: bold;
  position: absolute;
  --size: 25px;
  left: calc(-1 * var(--size) - 10px);
  line-height: var(--size);
  width: var(--size);
  height: var(--size);
  top: 0.3rem;
  border-radius: 50%;
  text-align: center;
}

.list{
    text-align:justify;
    /* display: inline-block; */
    position: absolute;
    left:15%;
    right:15%;
    top:30%;
}

    

</style>