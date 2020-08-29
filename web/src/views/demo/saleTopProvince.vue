<template>
  <div class="saleTopProvince">
    <div class="ranking-board-title">热销省份</div>
    <dv-charts :option="option1" />
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
      option1: {
        title: {
          text: "周销售额趋势",
        },
        xAxis: {
          name: "第一周",
          data: ["周一", "周二", "周三", "周四", "周五", "周六", "周日"],
          nameTextStyle: {
            fill: "#F8F8FF",
            fontSize: 10,
          },
          style: {
            stroke: "#4169E1",
            lineWidth: 1,
          },
        },
        yAxis: {
          name: "销售额",
          data: "value",
        },
        series: [
          {
            data: [1200, 2230, 1900, 2100, 3500, 4200, 3985],
            type: "bar",
            gradient: {
              color: ["#37a2da", "#67e0e3"],
            },
          },
        ],
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
  height: 50px;
  display: flex;
  align-items: center;
  font-size: 20px;
}
.saleTopProvince {
  position: relative;
  width: 100%;
  height: 49%;
  display: flex;
  justify-content: space-between;
  flex-shrink: 0;
  border: 1px solid green;
}
</style>