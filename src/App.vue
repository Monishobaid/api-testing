<script setup>
import BreakingBad from "./components/breakingBad.vue"
</script>

<template>
  <div>hello world main application</div>
  <Suspense>
    <template #default>
      <BreakingBad/>
    </template>
    <template #fallback>
     <p>loading...</p>
    </template>
  </Suspense>
</template>

<style scoped>
</style>
