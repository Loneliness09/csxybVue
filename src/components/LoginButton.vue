<script setup></script>
<template>
  <div style="display: flex; align-items: center">
    <a class="login">
      <div class="login_text">Login</div>
    </a>
  </div>
</template>

<style scoped>
.login {
  --font-family-text: Google Sans, Arial, Helvetica, sans-serif;
  font-family: var(--font-family-text);
  /* background: linear-gradient(90deg, #078efb 0, #ac87eb 66.7%); */
  box-sizing: border-box;
  display: inline-flex;
  align-items: center;
  gap: 8px;
  align-items: center;
  justify-content: center;
  white-space: nowrap;
  cursor: pointer;
  text-decoration: none;
  transition: all 0.3s ease;
  position: relative;
  border-radius: 60px;
  height: 60px;
  padding: 0 48px;
  color: #666;
  font-size: 20px;
  line-height: 24px;
  letter-spacing: 0.01em;
  overflow: hidden;
}

.login:hover::before {
  transform: translate(-50%);
  color: #fff;
}

.login::before {
  content: '';
  display: block;
  position: absolute;
  left: 0;
  width: 200%;
  top: 0;
  bottom: 0;
  border-radius: 60px;
  background: linear-gradient(60deg, rgb(42, 197, 161) 8%, #ac87eb 30%, #078efb 60%);
  transition: transform 0.5s ease;
  pointer-events: none;
  z-index: 1;
  transform: translate(0);
}

.login_text {
  font-family: var(--font-family-text);
  white-space: nowrap;
  cursor: pointer;
  color: #fff;
  letter-spacing: 0.01em;
  box-sizing: border-box;
  line-height: 1.5;
  font-weight: 500;
  position: relative;
  z-index: 2;
  font-size: 30px;
}
</style>
