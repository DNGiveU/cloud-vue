<template>
  <div class="index">
      </div class="nav">
        <Top class="top"></Top>
      </div>
      <!-- 组件显示位置 -->
      <router-view></router-view>
      <Footer></Footer>
  </div>
</template>

<script>

import Top from './top/';
import Footer from './footer/';

export default {
  components: { 
      Top, 
      Footer 
  },
  name: 'FrontIndex',
  data() {
      return {}
  },
  created() {},
  mounted() {},
  props: [],
  watch: {},
  computed: {},
  methods: {}
}
</script>

<style scoped>
.index {
    display: flex;
    padding: 0 0 20px 0;
    position: relative;
    min-height: 100%;
    background: #fff;
    overflow: hidden;
}

.nav {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    z-index: 999;
}

.top {
    margin-bottom: 2px;
}
</style>
