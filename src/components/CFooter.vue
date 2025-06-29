<!-- 底部组件 -->
<template>
  <footer class="number-footer">
    <div class="number-item" v-for="item in numberData" :key="item.id">
      <!-- 标题 -->
      <div class="title">{{ item.title }}</div>
      <!-- 数据 -->
      <div class="data">
        <img class="data-img" :src="item.img" alt="图标" />
        <div class="data-info">
          <!-- 数字 -->
          <div class="number">
            <span class="number-value">{{ item.value }}</span>
            <span class="number-unit">{{ item.unit }}</span>
          </div>
          <!-- 比较信息 -->
          <div class="compare">
            <span class="compare-label">较上年</span>
            <img class="compare-img" :src="item.compare === 'up' ? up : down" alt="上涨下跌图标" />
            <span
              class="compare-value"
              :style="{ color: item.compare === 'up' ? 'rgba(247, 61, 75, 1)' : 'rgba(11, 212, 167, 1)' }"
            >
              {{ item.proportion }}%
            </span>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<script setup lang="ts">
import { ref } from 'vue'
import 行李箱图标 from '@/assets/images/行李箱图标.png'
import 收入图标 from '@/assets/images/收入图标.png'
import 刷卡图标 from '@/assets/images/刷卡图标.png'
import up from '@/assets/images/up.png'
import down from '@/assets/images/down.png'
const numberData = ref<any>([
  {
    title: '2022年旅游业收入',
    value: 12345.6,
    unit: '万元',
    compare: 'down',
    proportion: 2.9,
    img: 收入图标
  },
  {
    title: '2022年来访游客数',
    value: 731.2,
    unit: '万人',
    compare: 'up',
    proportion: 1.6,
    img: 行李箱图标
  },
  {
    title: '2022年山东人口出游支出',
    value: 8373.1,
    unit: '万元',
    compare: 'down',
    proportion: 2.9,
    img: 刷卡图标
  }
])
</script>

<style lang="scss" scoped>
.number-footer {
  position: absolute;
  width: 100%;
  bottom: 55px;
  display: flex;
  justify-content: center;
  gap: 72px;
  pointer-events: none;
}
.number-item {
  position: relative;
  width: 268px;
  display: flex;
  flex-direction: column;
  gap: 16px;
  align-items: center;
  pointer-events: auto;
  .title {
    height: 35px;
    width: 100%;
    background: url('@/assets/images/titleBg.png') no-repeat center center;
    background-size: 100% 100%;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 16px;
  }
  .data {
    height: 82px;
    width: 100%;
    display: flex;
    gap: 28px;
    justify-content: center;
    .data-img {
      width: 82px;
      height: 82px;
    }
    .data-info {
      box-sizing: border-box;
      display: flex;
      flex-direction: column;
      justify-content: center;
      gap: 16px;
    }
    .number {
      display: flex;
      align-items: end;
      gap: 10px;
      .number-value {
        font-size: 32px;
        font-family: 'UniDreamLED';
        color: #fff;
        text-shadow: 0px 0px 13px rgb(154, 110, 44);
      }
      .number-unit {
        font-size: 14px;
        color: #fff;
      }
    }
    .compare {
      display: flex;
      align-items: center;
      gap: 10px;
      .compare-label {
        font-size: 14px;
        color: #c9d3ea;
        margin-right: 14px;
      }
      .compare-img {
        width: 20px;
        height: 12px;
      }
    }
  }
}
</style>
