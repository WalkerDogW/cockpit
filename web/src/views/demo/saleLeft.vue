<template>
  <div class="saleLeft">
    <!-- <div class="title">销售概况</div> -->
    <dv-border-box-8 class="title" :reverse="true">
      <div class="center-title">销售概况</div>
    </dv-border-box-8>
    <saleInfo class="saleInfo" />
    <saleCount class="saleCount" />
  </div>
</template>

<script>
import saleInfo from "./saleInfo";
import saleCount from "./saleCount";
export default {
  //import 引入的组件需要注入到对象中才能使用
  components: { saleInfo, saleCount },
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
.businessLeft {
  /* flex: 1; */
  display: flex;
  flex-direction: column;
}
.title {
  position: relative;
  width: 100%;
  height: 10%;
  display: flex;
  justify-content: space-between;
  flex-shrink: 0;
  border: 1px solid red;
}
.center-title {
  position: absolute;
  font-size: 30px;
  font-weight: bold;
  left: 50%;
  top: 5px;
  transform: translateX(-50%);
  color: RoyalBlue;
}
</style>