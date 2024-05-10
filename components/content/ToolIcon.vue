<script lang="ts" setup>
defineProps({
  icon: {
    type: String,
    required: true,
  },
  title: {
    type: String,
    default: "",
  }
})
</script>

<template>
  <img class="tool-icon" :src="icon" :title="title" />
</template>

<style scoped>
.tool-icon
{
    width: 40px;
    height: 40px;
    display: inline-block;
    margin: 5px;
}
</style>