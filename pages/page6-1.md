<!-- button -->
<p style="font-size:1.1rem">
  First, let's show how we preprocessing our data:
</p>
<div> 
  Step4, for each topic, we count both the number of negative and positive articles. Then we use min-max normalization on the both counts and assign (score<sub>pos</sub>, score<sub>neg</sub>).
  <div class="outbox mt-4rem mb-2rem">
    <div class="column">
      <img src="/img/EntitiesLink.jpg" style="width:100%">
    </div>
    <div class="column">
      <img src="/img/arrow1.svg" class = "arrow" >
    </div>
    <div class="column">
      <img src="/img/Topics_5.jpg" style="width:58%">
    </div>
  </div>
  <div > 
      <div class="absolute top-13rem left-49rem text-xs">
        <p>
            --> (<span class="pos_color">0.53</span>, <span class="neg_color">0.33</span>)
        </p>
      </div>
      <div class="absolute top-15.5rem left-49rem text-xs">
          <p>
            --> (<span class="pos_color">0.9</span>, <span class="neg_color">1.0</span>)
          </p>
      </div>
      <div class="absolute top-18rem left-49rem text-xs">
          <p>
              --> (<span class="pos_color">0.14</span>, <span class="neg_color">0.45</span>)
          </p>
      </div>
  </div>
</div>
<div v-after class="absolute left-40rem bottom-5rem">
    <div class="box absolute" >
        <span class="encode">
                how we encode our data?
        </span>
    </div>
	<div class="absolute left-10rem -bottom-1.4rem">
        <input class="modal-btn " type="checkbox" id="modal-btn" name="modal-btn"/>
      	<label for="modal-btn">Click me</label>
      	<div class="modal">		
	      	<div class="modal-wrap">	
				<img src="/img/6.jpg" alt="">	
	      		<p class="text-justify">We plot each topic using <span class="pos_color">score<sub>pos</sub></span> as x-coordinate and <span class="neg_color">score<sub>neg</sub></span> as y-coordinate on the 2-D scatter plot.</p>	          		
	      	</div>			          		
      	</div>	
	</div>
</div>



<style>
    @import url("https://use.fontawesome.com/releases/v5.5.0/css/all.css");
    .box{
        /* background-color: #3c3f41; */
        width: max-content;
        display: flex;
    }
    .encode{
        font-size: 13px;
        color: #000;
        overflow: hidden;
        /* border-right: 1px solid ; */
        white-space: nowrap;
        margin: 0 auto;
        animation:
            typing 1s steps(20),
            cursor 0.5s;
            /* cursor 0.5s step-end infinite; */
    }
    @keyframes typing {
        from{ width: 0 }
        to{ width: 100% }
    }
    /* @keyframes cursor{
        from, to {
            border-color: transparent;}
    
        50% {
        border-color: black;}
    } */
    /* .enter{
        text-align: center;
        border-radius: 15px;
        width: 4.5rem;
        line-height: 1.5rem;
        border:1px solid #fda4af;
        font-size: 13px;
        animation: clickit 1.5s
    } */
    @keyframes clickit {
        0% {opacity: 0}
        80% {opacity: 0}
        100% {opacity: 1}
    }
  .text-xs {
    font-size: 11px;
  }
  .outbox{
    display: flex;
    justify-content: center;
    align-items: center;
  }
  .column {
  float: left;
  width: 30%;
  padding: 1px;
  }
  .arrow{
    margin: auto;
    width:20%;
  }
  .neg_color{
    background: #f4c49c;
  }
  .pos_color {
    background: #baf0f5;
  }
p{
    font-weight: 400;
    font-size: 16px;
    line-height: 1.7;
    /* color: #1f2029; */
}

[type="checkbox"]:checked,
[type="checkbox"]:not(:checked){
  position: absolute;
  left: -9999px;
}
.modal-btn:checked + label,
.modal-btn:not(:checked) + label{
    border-radius: 16px;
    border:2px solid #fda4af;
    background-color:white;
    color:#fda4af;
    font-size: 12px;
    padding: 3px;
    width: 4rem;
    display: flex;
    justify-content: center;
    cursor: pointer;
    animation: clickit 1.5s
}
.modal-btn:not(:checked) + label:hover{
  background-color: #fda4af;
  color: white;
}

.modal-btn:checked + label:after,
.modal-btn:not(:checked) + label:after{
  position: fixed;
  top: 30px;
  right: 30px;
  z-index: 110;
  width: 35px;
  height: 25px;
  border-radius: 3px;
  background: white;
  color:#fda4af;
  display: flex;
  justify-content: center;
  font-size: 16px;
  content: "\f00d";
  font-weight: 600;
  font-family: "Font Awesome 5 Free";
  box-shadow: 0 12px 25px 0 rgba(16,39,112,.25);
  transition: all 200ms linear;
  opacity: 0;
  pointer-events: none;
  transform: translateY(20px);
}
.modal-btn:checked + label:hover:after,
.modal-btn:not(:checked) + label:hover:after{
  background-color: #fda4af;
  color: white;
}
.modal-btn:checked + label:after{
  transition: opacity 300ms 300ms ease, transform 300ms 300ms ease, background-color 250ms linear, color 250ms linear;
  opacity: 1;
  pointer-events: auto;
  transform: translateY(0);
}
.modal{
  position: fixed;
  /* display: block; */
  /* display: -ms-flexbox; */
  display: flex;
  /* -ms-flex-wrap: wrap; */
  /* flex-wrap: wrap; */
  /* -ms-flex-pack: center; */
  justify-content: center;
  /* margin: 0 auto; */
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  z-index: 100;
  overflow-x: hidden;
  background-color: rgba(31,32,41,.8);
  pointer-events: none;
  opacity: 0;
  transition: opacity 250ms 700ms ease;
}
.modal-btn:checked ~ .modal{
  pointer-events: auto;
  opacity: 1;
  transition: all 300ms ease-in-out;
}
.modal-wrap {
  position: relative;
  display: block;
  width: 100%;
  max-width: 400px;
  /* margin: 0 auto; */
  margin-top: 20px;
  margin-bottom: 20px;
  border-radius: 4px;
  overflow: hidden;
  /* padding-bottom: 20px; */
  background-color: #fff;
    /* -ms-flex-item-align: center; */
  align-self: center;
  box-shadow: 0 12px 25px 0 rgba(199,175,189,.25);
  opacity: 0;
  transform: scale(0.6);
  transition: opacity 250ms 250ms ease, transform 300ms 250ms ease;
}
.modal-wrap img {
  display: block;
  margin-left:auto;
  margin-right:auto;
  margin-top:16px;
  width: 100%;
  /* height: auto; */
}
.modal-wrap p {
  padding: 20px 30px 20px 30px;
  /* text-align:center; */
}
.modal-btn:checked ~ .modal .modal-wrap{
  opacity: 1;
  transform: scale(1);
  transition: opacity 250ms 500ms ease, transform 350ms 500ms ease;
}
</style>
