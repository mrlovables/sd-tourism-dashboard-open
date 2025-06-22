<!-- 顶部标题 -->
<template>
  <header class="header">山东省旅游指标监控平台</header>
</template>

<script setup lang="ts"></script>

<style lang="scss" scoped>
.header {
  position: absolute;
  margin: 0 12px;
  top: 12px;
  width: calc(100% - 24px);
  height: 87px;
  background: url('@/assets/images/顶部标题.png') no-repeat center center;
  background-size: 100% 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 40px;
  font-weight: 800;
  letter-spacing: 12px;
  color: rgba(230, 239, 253);
  font-family: 'MStiffHeiPRC';
}
</style>
