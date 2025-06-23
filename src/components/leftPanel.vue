<!-- 左侧数据面板 -->
<template>
  <div class="left-panel">
    <!-- 景点人流排名 -->
    <rankingOfScenicSpots />
  </div>
</template>

<script setup lang="ts">
import rankingOfScenicSpots from './leftPanel/rankingOfScenicSpots.vue'
</script>

<style lang="scss" scoped>
.left-panel {
  position: absolute;
  width: 500px;
  height: 100%;
  left: 38px;
  top: 111px;
}
</style>
