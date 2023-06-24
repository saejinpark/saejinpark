<style>
  .blind {
    overflow: hidden;
    position: absolute;
    clip-path: polygon(0 0, 0 0, 0 0, 0 0);
    width: 1px;
    height: 1px;
    margin: -1px;
  }
  .container {
    min-width: 480px;
    padding: 1rem;
    border: 1px solid black;
  }
  
  
  #info {
    border: 1px solid black;
    margin-bottom: 30px;
  }

  #info .inner {
    display: flex;
  }
  
  #info .inner .left {
    margin: 0;
    padding: 0;
    max-width: 120px;
    border: 1px solid black;
  }
  #info .inner .left img {
    object-fit: cover;
    height: 100%;
  }
  #info .inner .left figcaption {
    margin: 0;
    padding: 0;
  }
  
  #info .inner .right {
    width: 100%;
    padding: 1rem;
    border: 1px solid black;
  }
  
  #info .inner .right dl {
    margin: 0;
  }
  #info .inner .right dl dt{
    font-style: normal;
    margin: 0;
    display: inline-block;
    width: 60px;
    border: 1px solid black;
    text-align: right;
  }
  #info .inner .right dl dd {
    padding: 0;
    display: inline;
  }


  #tab-trigger-01:checked ~ #tabs .tab-list li:nth-child(1) .tab {
    background-color: gray;
  }
  
  #tab-trigger-02:checked ~ #tabs .tab-list li:nth-child(2) .tab {
    background-color: gray;
  }
  
  #tab-trigger-03:checked ~ #tabs .tab-list li:nth-child(3) .tab {
    background-color: gray;
  }
  
  #tab-trigger-04:checked ~ #tabs .tab-list li:nth-child(4) .tab {
    background-color: gray;
  }

  .panel {
    display: none;
    padding: 1rem;
  }


  #tab-trigger-01:checked ~ #tabs .panel-container #panel1 {
    display: block;
  }
  #tab-trigger-02:checked ~ #tabs .panel-container #panel2 {
    display: block;
  }
  #tab-trigger-03:checked ~ #tabs .panel-container #panel3 {
    display: block;
  }
  #tab-trigger-04:checked ~ #tabs .panel-container #panel4 {
    display: block;
  }

  #tabs {
    border: 1px solid black;
    display: flex;
  }

  #tabs .tab-list {
    display: inline-flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    margin: 0px;
    padding: 0;
  }

  #tabs .tab-list li {
    margin: 0px;
    padding: 0px;
    height: 100%;
    width: 120px;
    list-style-type: none;
  }

  #tabs .tab {
    display: flex;
    width: 100%;
    height: 100%;
    padding-left: 1rem;
  }
</style>

<div class="container">
  <input class="blind" type="radio" class="tab-trigger" name="tab-trigger" id="tab-trigger-01" checked/>
  <input class="blind" type="radio" class="tab-trigger" name="tab-trigger" id="tab-trigger-02"/>
  <input class="blind" type="radio" class="tab-trigger" name="tab-trigger" id="tab-trigger-03"/>
  <input class="blind" type="radio" class="tab-trigger" name="tab-trigger" id="tab-trigger-04"/>
  <div id="info">
    <div class="inner">
      <figure class="left">
        <img src="https://github.com/saejinpark/saejinpark/assets/54755633/70b0f4e1-2d50-4578-804b-71921c38deea"/>
        <figcaption class="blind">
          geppetto
        </figcaption>
      </figure>
      <div class="right">
        <dl>
          <dt>닉네임:</dt>
          <dd>geppetto</dd>
        </dl>
        <dl>
          <dt>분야:</dt>
          <dd>front-end</dd>
        </dl>
      </div>
    </div>
  </div>
  <div id="tabs">
    <aside>
      <nav>
        <ul class="tab-list">
          <li>
            <label class="tab" for="tab-trigger-01">introduce</label>
          </li>
          <li>
            <label class="tab" for="tab-trigger-02">education</label>
          </li>
          <li>
            <label class="tab" for="tab-trigger-03">experience</label>
          </li>
          <li>
            <label class="tab" for="tab-trigger-03">skill</label>
          </li>
          <li>
            <label class="tab" for="tab-trigger-04">portfolio</label>
          </li>
        </ul>
      </nav>
    </aside>
    <div class="panel-container">
      <section class="panel" id="panel1">
        <h2 class="blind">소개</h2>
        ㄹㅇㄴㅁㄹㅇㄴ
      </section>
      <section class="panel" id="panel2">
        <h2 class="blind">패널2</h2>
        <blockquote>
          <ul>
            <li>fdafd</li>
          <ul>
        </blockquote>
      </section>
      <section class="panel" id="panel3">
        <h2 class="blind">패널3</h2>
      </section>
      <section class="panel" id="panel4">
        <h2 class="blind">패널4</h2>
      </section>
    </div>
  </div>
</div>




