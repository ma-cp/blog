---
title: ma-cp的blog
---

吾生也有涯，而知也无涯。以有涯逐无涯，殆已！

<!-- 如果要添加新的一个标签，搜索关键字“添加新标签”，并按照搜索到的注释去更改 -->

<body>
<div class="warpper">
  <input class="radio" id="one" name="group" type="radio" checked>
  <input class="radio" id="two" name="group" type="radio">
  <input class="radio" id="three" name="group" type="radio">
<!-- 添加新标签：复制这两行模板，选择其中一个进行更改 -->
<!-- <input class="radio" id="{}" name="group" type="radio"> -->

  <div class="tabs">
  <label class="tab" id="one-tab" for="one">Programmer💻</label>
  <label class="tab" id="two-tab" for="two">Artist🎨</label>
  <label class="tab" id="three-tab" for="three">🤔</label>
  <!-- 添加新标签：复制这两行模板，选择其中一个进行更改 -->
<!-- <label class="tab" id="{}-tab" for="{}">新标签的标题</label> -->
    </div>
  <div class="panels">
  <div class="panel" id="one-panel">
    <div class="panel-title">精益求精</div>
    <p><a href="https://telegra.ph/%E8%AE%B0github-pages-02-17">记github-pages</a></p>
  </div>
  <div class="panel" id="two-panel">
    <div class="panel-title">虽有智慧，不如乘势。</div>
    <p></p>
  </div>
  <div class="panel" id="three-panel">
    <div class="panel-title">难免有些感想</div>
    <p></p>
  </div>
  <!-- 添加新标签：复制这两行模板，选择其中一个进行更改 -->
<!--
  <div class="panel" id="{}-panel">
    <div class="panel-title">新标签的内容标题</div>
    <p>内容</p>
  </div>
 -->

  </div>
</div>
</body>

<style>
    .warpper{
      display:flex;
      flex-direction: column;
      align-items: center;
    }
    .tab{
      cursor: pointer;
      padding:10px 20px;
      margin:0px 2px;
      display:inline-block;
      border-radius:3px 3px 0px 0px;
      box-shadow: 0 0.5rem 0.8rem #00000080;
    }
    .panels{
      background:#fffffff6;
      box-shadow: 0 2rem 2rem #00000080;
      min-height:200px;
      width:100%;
      max-width:500px;
      border-radius:3px;
      overflow:hidden;
      padding:20px;
    }
    .panel{
      display:none;
      animation: fadein .8s;
    }
    @keyframes fadein {
        from {
            opacity:0;
        }
        to {
            opacity:1;
        }
    }
    .panel-title{
      font-size:1.5em;
      font-weight:bold
    }
    .radio{
      display:none;
    }

/* 添加新标签：复制这两行模板，选择其中一个进行更改 */
/*
    #{}:checked ~ .panels #{}-panel,
*/
    #one:checked ~ .panels #one-panel,
    #two:checked ~ .panels #two-panel,
    #three:checked ~ .panels #three-panel{
      display:block
    }

/* 添加新标签：复制这两行模板，选择其中一个进行更改 */
/*
    #{}:checked ~ .tabs #{}-tab,
*/
    #one:checked ~ .tabs #one-tab,
    #two:checked ~ .tabs #two-tab,
    #three:checked ~ .tabs #three-tab{
      border-top: 3px solid #0b8b19;
    }
</style>