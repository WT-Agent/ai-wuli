<template>
  <div class="glass-card ticker-card">
    <div class="ticker-wrapper">
      <div v-for="(item, index) in tickerItems" :key="index" class="ticker-item">
        <span>{{ item.text }}</span>
        <span style="color: var(--success-color); font-weight: bold;">[生成完成]</span>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue';

const tickerItems = ref([
  {
    "text": "用户 136****5500 求解了带电粒子在交变电磁场中的偏转轨迹"
  },
  {
    "text": "用户 188****2211 获得了传送带物块滑动相对位移与热量求解"
  },
  {
    "text": "用户 131****4499 完成了双棒切割磁感线回路感应电量推导"
  },
  {
    "text": "用户 153****7722 生成了单摆小角度简谐运动周期公式证明"
  },
  {
    "text": "用户 177****1133 取得了高考物理 10 大模型受力分析思维导图"
  }
]);
</script>
