<template>
  <nav class="navbar">
    <ul class="nav-links">
      <li><router-link to="/">主页</router-link></li>
      <li><router-link to="/secondHandMarket">二手市场</router-link></li>
      <li><router-link to="/support">服务与支持</router-link></li>
      <li><router-link to="/about">关于我们</router-link></li>
      <li><router-link to="/download">APP下载</router-link></li>
    </ul>
  </nav>
</template>

<script>
import { RouterLink } from 'vue-router'
export default {
  methods: {
    login() {
      // 登录逻辑
    },
    register() {
      // 注册逻辑
    },
  },
}
</script>

<style scoped>
.navbar {
  width: auto;
  min-width: 1000px;
  background-color: #fff; /* 背景颜色 */
  padding: 10px 20px; /* 内边距 */
  display: flex;
  justify-content: space-around;
  align-items: center;
  flex-grow: 1;
  z-index: 1000;
}

.nav-links {
  list-style: none;
  display: flex;
  justify-content: space-around;
  width: 90%;
  padding: 0;
}

.nav-links li {
  position: relative;
}

.nav-links a {
  text-decoration: none;
  color: #333; /* 文字颜色 */
  font-weight: bold;
  font-size: xx-large;
  padding: 10px 32px;
  border-radius: 60px;
  border: 4px solid transparent;
  border-top: none;
  border-bottom: none;
}

.nav-links a.router-link-exact-active {
  border-color: var(--header-active-link-border-color);
}
.auth-buttons button {
  margin-left: 10px; /* 按钮之间的间隔 */
  padding: 5px 15px; /* 按钮的内边距 */
  border: none;
  background-color: #007bff; /* 按钮背景颜色 */
  color: #fff; /* 按钮文字颜色 */
  cursor: pointer;
  border-radius: 5px; /* 圆角 */
}

.auth-buttons button:hover {
  background-color: #0056b3; /* 鼠标悬停时的背景颜色 */
}
</style>
