<template>
  <div class="concent">
    <div>
      home组件
    </div>
    <div>
      <el-button type="info" @click="logout">退出</el-button>
    </div>
  </div>
</template>

<script>
export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: 'Home',
  methods: {
    logout () {
      window.sessionStorage.clear()
      this.$router.push('./login')
    }

  }
}
</script>

<style lang="less" scoped>

</style>
