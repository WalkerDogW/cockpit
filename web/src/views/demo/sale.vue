<template>
  <div class="sale">
      <saleLeft class="saleLeft"/>
      <saleMiddle class="saleMiddle"/>
      <saleRight class="saleRight"/>
  </div>
</template>

<script>
import saleLeft from "./saleLeft";
import saleMiddle from "./saleMiddle";
import saleRight from "./saleRight";
export default {
  //import 引入的组件需要注入到对象中才能使用
  components: { saleLeft, saleMiddle, saleRight },
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
.sale {
  position: relative;
  width: 100%;
  height: 49%;
  display: flex;
  justify-content: space-between;
  flex-shrink: 0;
  border:1px solid blue;
}
.saleLeft {
  width: 33%;
  height: 100%;
  border:1px solid khaki;
}
.saleMiddle {
  width: 33%;
  height: 100%;
  border:1px solid pink;
}
.saleRight {
  width: 33%;
  height: 100% ;
  border:1px solid lightgrey;
}
</style>