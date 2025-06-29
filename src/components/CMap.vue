<!--  中间地图部分 -->
<template>
  <div class="map">
    <CEcharts :option="mapOption" />
  </div>
</template>

<script setup lang="ts">
import { ref } from "vue";
import { getMapOption } from "@/modules/echartMap";
import CEcharts from "./common/CEcharts.vue";
const mapOption = ref(getMapOption());
</script>

<style lang="scss" scoped>
.map {
  position: relative;
  width: 100%;
  height: 100%;
}
</style>
