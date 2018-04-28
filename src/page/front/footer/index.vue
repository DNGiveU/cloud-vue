<template>
  <div class="footer">
    <!-- 相关链接 e.g. github gitee -->
    <div class="top">
        <span v-for="(item, index) in links" :key="index">
            <a :href="item.href" target="_blank">{{ item.label }}</a>
        </span>
    </div>
    <!-- 个人信息 -->
    <div class="bottom">
       {{ motto }} Power by {{ organization }} © {{ currentDate | parseTime('{y}') }} {{ author }}
    </div>
  </div>
</template>

<script>
export default {
  components: {},
  name: 'Footer',
  data() {
      return {
          links: [], // { href, label }
          currentDate: new Date(),
          motto: '欠一个座右铭...',
          organization: 'Cloud',
          author: 'gaz'
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
.footer {
    text-align: center;
    .top {

    }
    .bottom {

    }
}
</style>
