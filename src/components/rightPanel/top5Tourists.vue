<!-- 接待游客人数TOP5 -->
<template>
  <CPanel>
    <template #header>接待游客人数TOP5</template>
    <template #content>
      <CEcharts :option="option" />
    </template>
  </CPanel>
</template>

<script setup lang="ts">
import { ref, onMounted } from 'vue'
import * as echarts from 'echarts'
import CPanel from '@/components/common/CPanel.vue'
import CEcharts from '@/components/common/CEcharts.vue'

const option = ref<any>({})
const createEchartBar = () => {
  return {
    /**区域位置*/
    grid: {
      left: '3%',
      right: '4%',
      bottom: '3%',
      containLabel: true
    },
    tooltip: {
      trigger: 'axis'
    },
    xAxis: {
      type: 'category',
      data: ['青岛市', '济南市', '烟台市', '威海市', '潍坊市'],
      axisLine: {
        show: false
      },
      axisTick: {
        show: false
      },
      axisLabel: {
        color: '#C5D6E6',
        fontSize: 12
      }
    },
    yAxis: {
      axisLine: {
        show: false
      },
      splitLine: {
        lineStyle: {
          color: 'rgba(52, 71, 112, 1)',
          type: 'dashed'
        }
      },
      axisLabel: {
        color: '#C5D6E6',
        fontSize: 14
      },
      axisTick: {
        show: false
      }
    },
    series: [
      {
        name: '数(人次)',
        type: 'pictorialBar',
        barWidth: '150%',
        symbol: 'path://M0,10 L10,10 C5.5,10 5.5,5 5,0 C4.5,5 4.5,10 0,10 z',
        itemStyle: {
          normal: {
            opacity: 0.8,
            color: new echarts.graphic.LinearGradient(
              0,
              1,
              0,
              0,
              [
                {
                  offset: 0,
                  color: 'rgba(94, 111, 153, 0.2)' // 0% 处的颜色
                },
                {
                  offset: 0.6,
                  color: 'rgba(94, 111, 153, 0.8)' // 60% 处的颜色
                },
                {
                  offset: 1,
                  color: 'rgba(94, 111, 153, 1)' // 100% 处的颜色
                }
              ],
              false
            ),
            borderColor: 'rgba(109, 128, 175, 1)', // 边框颜色
            borderWidth: 4, // 边框宽度
            borderRadius: [100, 100]
          },
          emphasis: {
            color: new echarts.graphic.LinearGradient(
              0,
              1,
              0,
              0,
              [
                {
                  offset: 0,
                  color: 'rgba(218, 163, 88, 0.3)' // 0% 处的颜色
                },
                {
                  offset: 0.6,
                  color: 'rgba(218, 163, 88, 0.8)' // 60% 处的颜色
                },
                {
                  offset: 1,
                  color: 'rgba(218, 163, 88, 0)' // 100% 处的颜色
                }
              ],
              false
            ),
            borderColor: 'rgba(218, 163, 88, 1)' // 边框颜色
          }
        },
        data: [123, 100, 125, 100, 125],
        z: 10
      }
    ]
  }
}
onMounted(() => {
  option.value = createEchartBar()
})
</script>
<style lang="scss" scoped></style>
