<template>
  <div class="content">
    <h1>Content</h1>
    <img src="../../assets/vue.svg">
    <br>
    <n-button type="primary" @click="store.increment">
      {{ store.count }}
    </n-button>
  </div>
</template>

<script setup lang="ts">
import { NButton } from 'naive-ui'
import { useCounterStore } from '../store/counter'
const store = useCounterStore()
</script>

<style scoped lang="less">
.content {
  padding: 10px;
  background-color: #fff;
  box-shadow: 0 2px 12px 0 rgba(0, 0, 0, .1);
  border: 1px solid #ebeef5;
}
</style>