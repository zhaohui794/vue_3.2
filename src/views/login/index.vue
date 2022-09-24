<template>
  <div class="login-container">
    <el-form ref="form" :model="form">
      <el-form-item>
        <el-input v-model="form.name"></el-input>
      </el-form-item>
      <el-form-item>
        <el-button type="primary" @click="onSubmit">立即创建</el-button>
        <el-button>取消</el-button>
      </el-form-item>
    </el-form>
  </div>
</template>

<script setup>
import { ref } from 'vue'
const form = ref({
  name: ''
})
</script>

<style lang="scss" scoped>
.login-container {
}
</style>
