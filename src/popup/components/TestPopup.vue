<template>
  <div class="pop-container">
    <n-button @click="handleClick('导航1')">
      导航1
    </n-button>
    <n-button type="primary" @click="handleClick('导航2')">
      导航2
    </n-button>
    <n-button type="info" @click="handleClick('导航3')">
      导航3
    </n-button>
  </div>
</template>

<script setup lang="ts">
import { NButton, createDiscreteApi } from 'naive-ui'
const handleClick = (value: any) => {
  const { message } = createDiscreteApi(["message"])
  message?.info(value)
}
</script>

<style scoped lang="less">
.pop-container {
  min-width: 240px;
  padding: 10px;
  border-radius: 4px;

  .n-button {
    margin: 0 4px 0 0;
  }
}
</style>