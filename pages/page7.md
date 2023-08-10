<div>
  <div class="outbox" >
      <h1 class="absolute textbox" style="text-align: justify;">
        <span class="textword">
          Your journey with our system starts now! Click and Try out <span style="font-style: italic">NOVA</span> by youself ! <carbon:arrow-right class="inline"/>
          <img src="/img/nova_logo.png" class="h-10 mt-0.3rem mr-1rem cursor-pointer zoom"  style="float:right"
          @click="$slidev.nav.next"
          > 
        </span>
      </h1>
  </div>
</div>

<style>

div.slidev-layout.default.background.slidev-page.slidev-page-8{
  position: relative;
}
div.slidev-layout.default.background.slidev-page.slidev-page-8::after{
  content: '';
  position: absolute;
  inset: 0;
  z-index: -1;
  opacity: .1;
  background-image: url('/img/bg.jpg');
  background-size: cover;
  background-position: center;
}
.outbox{
  display: flex;
  justify-content: center;
  align-items: center;
}
.slidev-layout h1{
  background-color: #fff7ed;
  /* border-radius: 1.5rem; */
  color: #000;
  display: inline;
  font-size: 35px;
  line-height: 2;
}
.textbox .textword{
  background-color: #fff7ed;
  display: inline-block;
  line-height: 2;
  margin: 10px;
  padding: 30px;
}
.textbox{
    width: 800px;
    top:30%;
}
.zoom{
  transition: transform .2s;
}
.zoom:hover{
  transform: scale(1.3);
}
</style>