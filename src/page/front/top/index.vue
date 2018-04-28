<template>
  <div class="top">
    <!-- logo -->
    <img :src="logo" alt="logo" class="logo"/>
    <el-row>
      <el-col :span="1" v-for="(item, index) in topMenus" :key="index">
        <router-link :to="item.href">{{ item.label }}</router-link>
      </el-col>
    </el-row>
  </div>
</template>

<script>
import topMenus from '@/const/menu/front/';
export default {
  components: {},
  name: 'Top',
  data() {
      return {
        logo: 'https://avatars1.githubusercontent.com/u/6128107?v=4'
      }
  },
  created() {},
  mounted() {},
  props: [],
  watch: {},
  computed: {},
  methods: {}
}
</script>

<style lang="scss" scoped>
.top {
  .logo {
    width: 48px;
    height: 48px;
    border-radius: 50%;
  }
}
</style>

