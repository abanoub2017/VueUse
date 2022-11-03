<script setup>
import { useDark, useToggle } from '@vueuse/core';
const isDark = useDark();
const toggleDark = useToggle(isDark);
</script>

<template>
  <div>
    {{ isDark }}
  </div>
  <button @click="toggleDark()">Is Dark: {{ isDark }}</button>
</template>

<style>
.dark {
  background: #252525;
  color: #fff;
}
</style>
