<template>
  <div class="dark">
    <div class="bg-white shadow dark:bg-gray-700">
      <Header/>
      <div class="m-2 p-4 bg-gray-900 min-h-fit">
        <slot/>
      </div>
      <Footer/>
    </div>
  </div>
</template>
<script setup lang="ts">
</script>