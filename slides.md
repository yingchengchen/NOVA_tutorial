---
theme: seriph
background: background
class: text-center
lineNumbers: false
transition: side-right
title: NOVA Tutorial
---
<img class="bg" background-image src='/img/bg.jpg'/>
<div class="outbox -mt-5rem">
  <div class="column">
    <img src="/img/NOVA.jpg" class="h-70" style="margin:auto">
  </div>
  <div class="pt-12 absolute text">
    <span @click="$slidev.nav.next" class="px-2 py-1 rounded cursor-pointer text-black" hover="bg-black bg-opacity-10" style="font-style: italic">
      Press here or press &#x25B7 on the keyboard to start the tutorial
    </span>
  </div>

</div>

<style> 
.bg{
  opacity:0.06;
  position:absolute;
  left:0;
  top:0;
  width:100%;
  height:auto;
}
div.slidev-layout.cover.text-center.text-center.slidev-page.slidev-page-1{
  background: none !important;
}
  .outbox{
    display: flex;
    justify-content: center;
    align-items: center;
 }
  .column {
  /* float: left; */
  width: 100%;
  /* padding: 1px; */
}
  .text{
    bottom: 5rem;
    font-size: 0.8rem;
    
  }
</style>

---
src: /pages/page1.md
transition: side-right
layout: center
class: background
---
<!-- this page will be loaded from './pages/page1.md' -->
---
src: /pages/page2.md
transition: fade-out
class: background
preload: false
---
<!-- this page will be loaded from './pages/page2.md' -->
---
src: /pages/page3.md
transition: fade-out
class: background
preload: false
---
<!-- this page will be loaded from './pages/page3.md' -->
---
src: /pages/page4.md
transition: fade-out
class: background
preload: false
---
<!-- this page will be loaded from './pages/page4.md' -->
---
src: /pages/page5.md
transition: fade-out
class: background
preload: false
---
<!-- this page will be loaded from './pages/page5.md' -->
---
src: /pages/page6.md
transition: slide-up
class: background
preload: false
---
<!-- this page will be loaded from './pages/page6.md' -->
---
src: /pages/page7.md
transition: fade-out
class: background
preload: false
---
<!-- this page will be loaded from './pages/page7.md' -->
---

