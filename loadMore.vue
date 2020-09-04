<template>
  <div v-loadmore="loadmore">
    <div class="outBox">
      <li v-for="item in num">8888</li>
    </div>
  </div>
</template>

<script>
export default {
  components: {},
  props: {},
  data() {
    return {
      num: 10
    };
  },
  watch: {},
  computed: {},
  methods: {
    loadmore() {
      this.num += 10;
    }
  },
  created() {},
  mounted() {}
};
</script>
<style lang="scss" scoped>
.outBox {
  height: 100px;
  width: 100px;
  overflow: auto;
}
</style>