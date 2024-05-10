<script lang="ts" setup>
import { ref } from 'vue';

defineProps({
  title: {
    type: String,
    default: "",
  }
})

let show = ref(false);

</script>

<template>
  <UCard>
    <template #header>
      {{title}}
    </template>

    <Placeholder class="h-32" />

    <template #footer>
      <Placeholder class="h-8" />
    </template>
  </UCard>
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