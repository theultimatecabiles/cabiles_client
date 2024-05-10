<template>
  <div class="centered-layout">
    <slot></slot>
  </div>
</template>

<style scoped>
.centered-layout {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh; 
  font-size: 2.5rem; 
}
</style>