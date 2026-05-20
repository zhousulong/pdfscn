<template>
  <n-grid cols="1 m:2" x-gap="25px" y-gap="25px" responsive="screen" class="preview-grid">
    <n-grid-item class="preview-grid-item">
      <slot name="pdf" />
    </n-grid-item>
    <n-grid-item class="preview-grid-item">
      <slot name="scan" />
    </n-grid-item>
  </n-grid>
</template>

<script lang="ts" setup>
import { NGrid, NGridItem } from 'naive-ui'
</script>

<style scoped>
.preview-grid {
  width: 100%;
}
.preview-grid-item {
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
