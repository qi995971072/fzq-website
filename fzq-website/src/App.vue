<template>
  <div id="app">
    <div class="header">
      <!--<div class="header-image">-->
      <!--</div>-->
      <img src="./assets/test-header.png">
      <div style="padding-left: 15%; padding-right: 15%; box-sizing: border-box">
        <div class="menu">
          <div class="menu-item" v-for="item in menu_items">
            <img src="./assets/test-menu-icon.png"/>
            <div class="menu-title-container">
              <div v-for="(value, index) in item">
                <span v-if="index == 1" class="menu-title-big">{{value}}</span>
                <span v-else class="menu-title">{{value}}</span>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <router-view/>
    <div class="foot">
      <div class="foot-subscribe">
        <span style="border: solid 1px red">留下您的信息，订阅我们最新资讯</span>
        <div style="border: solid 1px red">资讯订阅</div>
      </div>
      <div class="foot-contactus">
        <div class="foot-contactus-item"></div>
        <div class="foot-contactus-item"></div>
        <div class="foot-contactus-item"></div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'App',
  data () {
    return {
      menu_items: [
        ['关于我们', 'Whe We Are', '使命*愿景', '义工*招募', '合作*伙伴', '意见*联系'],
        ['服务对象', 'Service Object', '寺庙*师父', '学佛弟子', '居士群主', '善士信众', '使用帮助'],
        ['核心功能', 'What We Do', '手机佛堂', '个人功课', '法本*课诵', '共修报数', '天天随喜'],
        ['共修*活动', 'Practice', '每天手机供佛', '共修报数', '今天我吃素', '广种福田', '行走的力量', '手机祈福']
      ]
    }
  }
}
</script>

<style lang="stylus">
#app {
  /*font-family: 'Avenir', Helvetica, Arial, sans-serif;*/
  /*-webkit-font-smoothing: antialiased;*/
  /*-moz-osx-font-smoothing: grayscale;*/
  /*text-align: center;*/
  /*color: #2c3e50;*/
  /*margin-top: 60px;*/
}

  .header {
    display: flex;
    flex-direction: column;
  }
  .header-image {
    width: 100%;
    background-color: red;
  }
  .header img {
    width: 100%;
  }
  .menu {
    width: 100%;
    /*height: 80px;*/
    background-color: yellow;
    display: flex;
    flex-direction: row;
    justify-content: center;
  }
  .menu-item {
    width: 100%;
    background-color: white;
    /*border: solid 1px red;*/

    display: flex;
    flex-direction: column;
    justify-content: flex-start;
    align-items: center;
    flex-shrink: 1;
    flex-grow: 1;
    padding-top: 30px;
  }
  .menu-item img {
    width: 37%;
    /*height:w;*/
  }
  .menu-title-container {
     margin-top: 25px;
   }
  .menu-title-big {
    font-size: 21px;
    text-align: center;
    width: 100%;
    display: block;
    line-height: 45px;
  }
  .menu-title {
    font-size: 15px;
    text-align: center;
    width: 100%;
    display: block;
    line-height: 26px;
  }
  .foot {
    width: 100%;
    background-color: green;
  }
  .foot-subscribe {
    width: 100%;
    height: 120px;
    background-color: #C68045;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
  .foot-contactus {
    width: 100%;
    height: 320px;
    background-color: #35161B;
    display: flex;
    flex-direction: row;
    flex-wrap: nowrap;
  }
  .foot-contactus-item {
    height: 100%;
    width: 100%;
    border: solid 1px red;
  }

/**
* Eric Meyer's Reset CSS v2.0 (http://meyerweb.com/eric/tools/css/reset/)
* http://cssreset.com
*/

/*
html, body, div, span, applet, object, iframe,
h1, h2, h3, h4, h5, h6, p, blockquote, pre,
a, abbr, acronym, address, big, cite, code,
del, dfn, em, img, ins, kbd, q, s, samp,
small, strike, strong, sub, sup, tt, var,
b, u, i, center,
dl, dt, dd, ol, ul, li,
fieldset, form, label, legend,
table, caption, tbody, tfoot, thead, tr, th, td,
article, aside, canvas, details, embed,
figure, figcaption, footer, header,
menu, nav, output, ruby, section, summary,
time, mark, audio, video, input
{
  margin: 0;
  padding: 0;
  border: 0;
  font-size: 100%;
  font-weight: normal;
  vertical-align: baseline;
}*/

  html, body {
    margin: 0;
    padding: 0;
    border: 0;
    font-size: 100%;
    font-weight: normal;
    vertical-align: baseline;
  }
</style>
