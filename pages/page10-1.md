<img class="bg" background-image src='/img/bg.jpg'/>
<br>
<br>
<div> 
    <div class="box">
        Steps we suggest for user to do in <span font-style: italic>Belief </span>page: 
        <img src="/img/Belief.jpg" class="h-15" style="float:right">
    </div>
    <div class="container">
        <ol class="list">
            <li>Build your own belief on the chosen topic and its highly-related topics on the hexagon. What do you think the outlet's perspective on them, negative, positive, neutral or mixed?</li>
            <li>Compare the one you have built to the hexagon generated based on our data. NOVA will help you highlight the differences between the two.</li>
            <li>Does the outlet report the topic more negative or positive than you expect? Pick one conflict topic and find out the reasons in the next page!</li>
        </ol>
    </div>
</div>
    <!-- After choosing the topic and the outlet the user wants to explore, we let user build their own belief and compare with what our data suggested. NOVA will then hughlight topics where users and data hold different perspectives.  -->



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