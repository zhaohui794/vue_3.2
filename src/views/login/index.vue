<template>
  <div class="login-container">
    <el-form ref="form" :model="form">
      <div class="title-container">
        <h3 class="title">用户登录</h3>
      </div>
      <el-form-item>
        <i class="el-icon-edit-outline" size="20"></i>
        <el-input v-model="form.name" placeholder="请输入账号"></el-input>
      </el-form-item>
      <el-form-item>
        <i class="el-icon-edit-outline" size="20"></i>
        <el-input
          v-model="form.name"
          show-password
          placeholder="请输入密码"
        ></el-input>
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
