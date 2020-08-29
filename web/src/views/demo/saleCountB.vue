<template>
  <div class="saleCountB">
    <transition name="el-zoom-in-center">
      <div v-show="show2" class="transition-box">.el-zoom-in-center</div>
    </transition>

    <transition name="el-zoom-in-top">
      <div v-show="show2" class="transition-box">.el-zoom-in-top</div>
    </transition>

    <transition name="el-zoom-in-bottom">
      <div v-show="show2" class="transition-box">.el-zoom-in-bottom</div>
    </transition>
  </div>
</template>

<script>
export default {
  //import 引入的组件需要注入到对象中才能使用
  components: {},
  props: {},
  data() {
    //这里存数据
    return {
      show2: false,
      items: [
        {
          title: "促销收入",
          number: 1300,
          unit: "万元",
        },
        {
          title: "促销订单数量",
          number: 586,
          unit: "万元",
        },
        {
          title: "促销产品总重量",
          number: 2510,
          unit: "万元",
        },
      ],
    };
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
  mounted() {
    this.show2 = true;
  },
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
.saleCountB {
  position: relative;
  width: 100%;
  height: 40%;
  display: flex;
  justify-content: space-between;
  flex-shrink: 0;
}
.transition-box {
  margin: 3% 0 3% 3%;
  /* margin-top: 3%;
  margin-left: 3%; */
  border-radius: 4px;
  text-align: center;
  color: #fff;
  padding: 40px 20px;
  box-sizing: border-box;
  margin-right: 20px;
  border: solid 1px cyan;
  width: 30%;
}
</style>