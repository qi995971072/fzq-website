<template>
  <div class="firstpage">
    <!--<div class="aboutus-item">-->
      <!--<span class="item-title">关于我们</span>-->
      <!--<div class="aboutus">-->
        <!--<div class="left-content">-->
          <!--<div>-->
            <!--<span class="left-content-title">使命*愿景</span>-->
            <!--<span>佛子圈app, 是一群志同道合的学佛者, 一起开发的一款免费佛教修行工具APP. 目标是创建一个综合性的佛教移动服务平台, 为佛教事业贡献自己绵薄之力</span>-->
          <!--</div>-->
          <!--<hr/>-->
          <!--<div>-->
            <!--<span style="display: block">招募*义工</span>-->
            <!--<ul>-->
              <!--<li>各地弘法平台专员</li>-->
              <!--<li>修行指导专员 - 各特定教派或传承</li>-->
              <!--<li>新媒体运营经理</li>-->
              <!--<li>活动策划专员</li>-->
              <!--<li>客服专员</li>-->
            <!--</ul>-->
          <!--</div>-->
          <!--<hr/>-->
          <!--<div>-->
            <!--<span style="display: block">合作*伙伴</span>-->
            <!--<ol>-->
              <!--<li>平台合作, 资源共享, 弘法利生, 共同进步</li>-->
              <!--<li>共同发起丰富多彩的共修、公益慈善、募捐活动</li>-->
            <!--</ol>-->
          <!--</div>-->
          <!--<hr/>-->
          <!--<div>-->
            <!--<span style="display: block">意见*联系</span>-->
            <!--<span style="display: block">疑问：App的使用方面有任何疑问请联系：</span>-->
            <!--<span style="display: block">cs@58fo.com</span>-->
          <!--</div>-->
        <!--</div>-->
        <!--<div class="aboutus-right-img">-->
          <!--&lt;!&ndash;<img src="../assets/test-header.png"/>&ndash;&gt;-->
        <!--</div>-->
      <!--</div>-->
    <!--</div>-->

    <div class="serviceObj">
      <span class="item-title">服务对象</span>
      <div style="display: flex; flex-direction: row">
        <div class="serviceObj-leftimg">
          <img src="../assets/test-header.png"/>
        </div>
        <div class="serviceObj-rightitems">
          <span v-for="item in ['寺庙*师父', '学佛弟子', '居士群主', '善士信众', '常见问题']" class="serviceObj-rightitems-item">
            {{item}}
          </span>
          <!--<div class="serviceObj-rightitems-item">寺庙*师父</div>-->
          <!--<div class="serviceObj-rightitems-item">学佛弟子</div>-->
          <!--<div class="serviceObj-rightitems-item">居士群主</div>-->
          <!--<div class="serviceObj-rightitems-item">善士信众</div>-->
          <!--<div >使用帮助</div>-->
        </div>
      </div>
    </div>

    <div>
      <span style="display: block; text-align: center">核心功能</span>
      <div>
        <img src="../assets/test-header.png"/>
      </div>
      <div>
        <img src="../assets/test-career-nav.png"/>
      </div>
    </div>

    <div>
      <span style="display: block; text-align: center;">共修活动</span>
      <div class="gxhd-itemcontaner">
        <div class="gxhd-itemcontaner-row">
          <div class="gxhd-item">
            <img src=""/>
            <span>每天手机供佛</span>
          </div>
          <div class="gxhd-item">
            <img src=""/>
            <span>共修报数</span>
          </div>
          <div class="gxhd-item">
            <img src=""/>
            <span>今天我吃素</span>
          </div>
        </div>
        <div class="gxhd-itemcontaner-row">
          <div class="gxhd-item">
            <img src=""/>
            <span>广种福田</span>
          </div>
          <div class="gxhd-item">
            <img src=""/>
            <span>行走的力量</span>
          </div>
          <div class="gxhd-item">
            <img src=""/>
            <span>手机祈福</span>
          </div>
        </div>
      </div>
    </div>

  </div>
</template>

<script>
export default {
  name: 'FirstPage',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .firstpage {
    margin-top: 50px;
    width: 100%;
  }
  .aboutus-item {
    padding-left: 15%;
    padding-right: 15%;
    box-sizing: border-box;
  }
  .item-title {
    display: block;
    text-align: center;
    font-size: 25px;
    line-height: 60px;
    /*background-color: red;*/
  }
  .aboutus {
    display: flex;
    flex-direction: row;
    /*background-color: red;*/
    justify-content: flex-start;
    align-items: stretch;
  }
  .left-content {
    /*width: 300px;*/
    background-color: white;
    font-size: 14px;

    flex-shrink: 0;
    flex-grow: 0;
    flex-basis: 250px;

    margin-right: 20px;
  }
  .left-content-title {
    display: block;
    line-height: 35px;
  }
  .aboutus-right-img {
    background-color: peachpuff;
    flex: 1;
    /*flex-grow: 1;*/
    /*flex-shrink: 1;*/
    /*height: 100%;*/
  }
  /*.aboutus img {*/
    /*width: 100%;*/
    /*flex-grow: 1;*/
    /*flex-shrink: 1;*/
  /*}*/

  .serviceObj {
    padding-left: 15%;
    padding-right: 15%;
    box-sizing: border-box;
    background-color: #FAF3E3;
  }
  .serviceObj-leftimg {
    width: 80%;
  }
  .serviceObj-leftimg img {
    width: 100%;
    height: 100%;
  }
  .serviceObj-rightitems {
    width: 20%;
  }
  .serviceObj-rightitems-item {
    width: 100%;
    height: 20%;
    background-color: green;
    text-align: center;
    border: solid 1px red;
    box-sizing: border-box;
    display: block;
  }
  .gxhd-itemcontaner {
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
    align-items: center;

    padding-left: 10%;
    padding-right: 10%;
    box-sizing: border-box;
  }
  .gxhd-itemcontaner-row {
    width: 100%;
    display: flex;
    flex-direction: row;
    flex-wrap: nowrap;
    justify-content: space-around;
  }
  .gxhd-item {
    width: 100%;
    height: 200px;
    background-color: green;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    border: solid 1px white;

    margin-left: 10px;
    margin-right: 10px;

    flex-shrink: 1;
    flex-grow: 1;
  }
  .gxhd-item img {
    width: 100%;
    height: 80%;
    background-color: red;
  }
</style>
