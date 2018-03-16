<template>
  <div>
    <div class="opacity-demo">
      <touchable-opacity class="back-icon-wrap">
        <img src="demo/assets/back.png" class="back-icon">
      </touchable-opacity>
      <touchable-opacity class="setting-icon-wrap">
        <img src="demo/assets/setting.png" class="settings-icon">
      </touchable-opacity>
    </div>

    <touchable-highlight>
      <div class="highlight-demo">
        <div class="wb-top">
          <img src="https://tvax4.sinaimg.cn/crop.0.0.200.200.180/75b1a75fly1fmfz7qvv75j205k05kt8p.jpg" class="wb-avatar">
          <div>
            <h3>环球时报</h3>
            <h4>10分钟前 来自 小米Mix2</h4>
          </div>
        </div>

        <div class="wb-content">
          【看广告不如“玩广告”】据外媒报道，谷歌将会在下周 GDC 大会上正式推出新型的“奖励广告”服务，将大部分广告制作成了可以玩的“小游戏”，其他视频广告也变成了可以自由挑选播放的形式。 ​
        </div>
      </div>
    </touchable-highlight>
  </div>
</template>

<script>
// import TouchableOpacity from '../src/TouchableOpacity'
// import TouchableHighlight from '../src/TouchableHighlight'
import { TouchableOpacity, TouchableHighlight } from '../dist/touchable'

export default {
  components: {
    TouchableOpacity,
    TouchableHighlight
  }
}
</script>

<style>
html, body, #app {
  margin: 0;
  width: 100%;
  height: 100%;
  background-color: #EFEFEF;
}

.opacity-demo {
  width: 100%;
  height: 40px;
  background-color: rgb(51, 137, 202);
  text-align: center;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.back-icon-wrap {
  display: flex;
  align-items: flex-end;
}

.wb-top {
  display: flex;
  padding-left: 0.7rem;
}

.wb-avatar {
  width: 2rem;
  height: 2rem;
  border-radius: 999px;
}

.wb-content {
  line-height: 1.5;
  word-wrap: break-word;
  text-align: left;
  color: #333;
  padding: 0.75rem 0.5rem 0.5rem 0.5rem;
}

h3, h4 {
  margin: 0;
  text-align: left;
  padding-left: 0.5rem;
}

h3 {
  font-size: .875rem;
  color: #333;
}

h4 {
  color: #939393;
  font-size: .6875rem;
}

.setting-icon-wrap {
  display: flex;
  align-items: flex-start;
}

.back-icon, .settings-icon {
  width: 20px;
  height: 20px;
}

.back-icon {
  margin-left: 10px;
}

.settings-icon {
  margin-right: 10px;
}

.highlight-demo {
  width: 100%;
  /*border: 1px solid #EEE;*/
  margin-top: 10px;
  padding-top: .75rem;
  text-align: center;
  background-color: #FFF;
}
</style>