<h1>Welcome to NOVA! </h1>
<div>
  <div class="textbox" style="text-align: justify">
    <span class="textword">
        NOVA, news outlet visual assessment, serves as a platform to allow general audiences to freely review mainstream media outlet coverage on a variety of topics. Additionally, our system supports user's in assessing if their prior expectations and understanding of an outlet aligns with how the iutlet reported on a selected topic.
    </span>
  </div>
  <div v-click>
    <div class="textbox" style="text-align: justify">
      <span class="textword">
          The article you will browse soon were centered around COVID-19 and collected from U.S. mainstream media outlets(New York Times, CNN, Fox News, Breitbart, Washington Post and ABC News) from Feb 2020 to June 2020.
      </span>
    </div>
    <div>
      <div class = "column">
        <img src="/img/New York Times.png" class="ml-2 mr-2 h-24" />
      </div>
      <div class = "column">
        <img src="/img/CNN.png" class="ml-2 mr-2 h-25" />
      </div>
      <div class = "column">
        <img src="/img/FoxNews.png" class="ml-2 mr-2 h-25" />
      </div>
      <div class = "column">
        <img src="/img/Breitbart.png" class="h-25" />
      </div>
      <div class = "column">
        <img src="/img/Washington Post.png" class="ml-2 mr-2 h-25" />
      </div>
      <div class = "column">
        <img src="/img/ABC News.png" class=" ml-2 mr-2 h-27" />
      </div>
    </div>
  </div>
</div>

<style>
div.slidev-layout.center.h-full.grid.place-content-center.background.slidev-page.slidev-page-2{
  position: relative;
}
div.slidev-layout.center.h-full.grid.place-content-center.background.slidev-page.slidev-page-2::after{
  content: '';
  position: absolute;
  inset: 0;
  z-index: -1;
  opacity: .1;
  background-image: url('/img/bg.jpg');
  background-size: cover;
  background-position: center;
}
.textbox{
  background-color: #fff7ed;
  color: #000;
  display: inline;
}
.textbox .textword{
  /* border-radius: 1.5rem; */
  background-color: #fff7ed;
  display: inline-block;
  /* line-height: 2; */
  margin: 10px;
  padding: 20px;
}

.column{
  float: left;
  width:16%;
  /* padding: 5px; */
}

.slidev-layout h1{
 color: black;
 margin-top: 3rem;
 /* margin-bottom: 1rem; */
 margin-left: 0rem;
}
</style>