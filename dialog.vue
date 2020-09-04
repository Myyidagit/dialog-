<template>
  <div v-dialogDrag class="outBox">
    <div class="m_dialog">
      <div class="dialog_header" :class="{'m-center':center}">
          我是标题
      </div>
      <div class="dialog_body"></div>
    </div>
  </div>
</template>

<script>
export default {
  components: {},
  props: {
      center:{
          type:Boolean,
          default:true
      }
  },
  data() {
    return {};
  },
  watch: {},
  computed: {},
  methods: {},
  created() {},
  mounted() {}
};
</script>
<style lang="scss" scoped>
.m-center{
    text-align: center;
}
.outBox {
  position: fixed;
  z-index: 88;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: rgba(0, 0, 0, 0.2);
  .m_dialog {
    width: 500px;
    height: 300px;
    position: absolute;
    top: 50%;
    left: 50%;
    margin-left: -250px;
    margin-top: -150px;
    .dialog_body {
      height: 370px;
      width: 500px;
    //   border: 1px solid #F56C6C;
      background: #fff;
    }
    .dialog_header {
      height: 40px;
      line-height: 40px;
      width: 100%;
      background: #F56C6C;
    }
  }
}
</style>