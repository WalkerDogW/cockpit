<template>
  <div id="data-view">
    <dv-full-screen-container>
      <top-header />

      <div class="main-content">
        <business class="business"/>
        <div class="spaceLine"></div>
        <sale class="sale"/>
      </div>

    </dv-full-screen-container>
  </div>
</template>

<script>
import topHeader from "./topHeader";
import business from "./business";
import sale from "./sale";
export default {
  //import 引入的组件需要注入到对象中才能使用
  components: { topHeader, business, sale },
  props: {},
  data() {
    //这里存数据
    return {};
  },
  //计算属性
  computed: {},
  //监控data中数据变化
  watch: {},
  //方法
  methods: {},
  //声明周期 - 创建完成（可以访问当前this实例）
  created() {},
  //生命周期 - 挂载完成（可以访问DOM元素）
  mounted() {},
  beforeCreate() {}, //生命周期 - 创建之前
  beforeMount() {}, //生命周期 - 挂载之前
  beforeUpdate() {}, //声明周期 - 更新之前
  updated() {}, //生命周期 - 更新之后
  beforeDestroy() {}, //生命周期 - 销毁之前
  destroyed() {}, //生命周期 - 销毁之后
  activated() {}, //缓存keep-alive
};
</script>

<style scoped>
.spaceLine{
  width: 100%;
  height: 1%;
}
#data-view {
  width: 100%;
  height: 100%;
  background-color: #030409;
  color: #fff;
}
#data-view #dv-full-screen-container {
  background-image: url("/static/img/background01.png");
  /* background-image: url("/static/img/background02.jpg"); */
  
  background-size: 100% 100%;
  box-shadow: 0 0 3px blue;
  display: flex;
  flex-direction: column;
  /* opacity:0.8 */
}
#data-view .main-content {
  flex: 1;
  display: flex;
  flex-direction: column;
}
/*
#data-view .block-left-right-content {
  flex: 1;
  display: flex;
  margin-top: 20px;
}
#data-view .block-top-bottom-content {
  flex: 1;
  display: flex;
  flex-direction: column;
  box-sizing: border-box;
  padding-left: 20px;
}
#data-view .block-top-content {
  height: 55%;
  display: flex;
  flex-grow: 0;
  box-sizing: border-box;
  padding-bottom: 20px;
} */

/* .business{
  background-color:coral;
  width: 30%;
}
.business{
  background-color:lightblue;
  width: 70%;
} */
</style>