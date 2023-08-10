  <div class="content">
    <h2 style="background-color:red">Hero title</h2>
    <p>Hero description here</p>
  </div>


<style>
 div.slidev-layout.default.background.slidev-page.slidev-page-10{
    position: relative;
 }
 div.slidev-layout.default.background.slidev-page.slidev-page-10::after{
    content: '';
    position: absolute;
    inset: 0;
    z-index: -1;
    opacity: .1;
    background-image: url('/img/bg.jpg');
    background-size: cover;
    background-position: center;
 }
</style>