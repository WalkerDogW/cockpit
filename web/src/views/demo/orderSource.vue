<template>
  <div class="orderSource">
    <div class="title">
      <p>
        <span class="title-text">订单来源</span>
      </p>
    </div>
    <div v-for="item in orderItems" :key="item.title" class="items">
      <p class="items-number"><span class="items-number-text">{{item.number}}</span></p>
      <p class="items-title"><span class="items-title-text">{{item.title}}</span></p>
    </div>
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
      orderItems: [
        {
          title: "新客户数",
          number: 5,
        },
        {
          title: "期间下单客户数",
          number: 411,
        },
        {
          title: "有效客户数",
          number: 645,
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
.orderSource {
  position: relative;
  width: 100%;
  height: 45%;
  display: flex;
  justify-content: space-between;
  flex-shrink: 0;
  border: 1px solid green;
}
</style>