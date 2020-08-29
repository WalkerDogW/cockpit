<template>
  <div class="saleTopProductCommon">
    <div class="ranking-board-title">热销产品</div>
    <dv-scroll-ranking-board :config="config" class="scroll-board" />
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
      config: {
        data: [
          {
            name: "周口",
            value: 55,
          },
          {
            name: "南阳",
            value: 120,
          },
          {
            name: "西峡",
            value: 78,
          },
          {
            name: "驻马店",
            value: 66,
          },
          {
            name: "新乡",
            value: 80,
          },
        ],
        unit: "单位",
      },
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
.ranking-board-title {
  font-weight: bold;
  height: 30px;
  display: flex;
  align-items: center;
  font-size: 15px;
}
.saleTopProductCommon {
  display: flex;
  flex-direction: column;
  align-items: center; /****水平居中****/
  justify-content: center; /*垂直居中*/
}

.scroll-board {
  width: 80%;
  height: 100%;
}
</style>