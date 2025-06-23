<!-- 通用面板 -->
<template>
  <div class="panel">
    <div class="panel-header">
      <slot name="header">默认名称</slot>
    </div>
    <div class="panel-container">
      <slot name="container"></slot>
    </div>
  </div>
</template>

<script setup lang="ts"></script>

<style lang="scss" scoped>
.panel {
  position: relative;
  width: 472px;
  height: fit-content;
  &-header {
    position: relative;
    width: 100%;
    height: 50px;
    display: flex;
    flex-direction: column;
    background: url('@/assets/images/titleBg.png') no-repeat center center;
    font-size: 20px;
    text-align: center;
    line-height: 50px;
    letter-spacing: 2px;
  }
  &-container {
    position: relative;
    height: 120px;
    outline: red solid 1px;
  }
}
</style>
