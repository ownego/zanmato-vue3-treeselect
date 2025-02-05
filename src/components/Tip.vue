<script setup>
defineOptions({
  name: "vue3-treeselect--tip"
});

defineProps({
  type: {
    type: String,
    required: true
  },
  icon: {
    type: String,
    required: true
  }
});
</script>

<template>
  <div :class="`vue3-treeselect__tip vue3-treeselect__${type}-tip`">
    <div class="vue3-treeselect__icon-container">
      <span :class="`vue3-treeselect__icon-${icon}`" />
    </div>
    <span
      :class="`vue3-treeselect__tip-text vue3-treeselect__${type}-tip-text`">
      <slot></slot>
    </span>
  </div>
</template>
