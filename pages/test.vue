<template>
    <div>

    </div>
</template>

<script setup lang="ts">
// run eslint pages/test.vue
import { Label } from '@/types/file'

withDefaults(
    defineProps<{
        label1?: string | Label
        label2?: string | Label
    }>(),{
    label1: () => ({ label: 'label', plural: true }),
    label2: () => {
        return { label: 'label', plural: true }
    }
  }
)
</script>

<style lang="scss" scoped>
</style>b