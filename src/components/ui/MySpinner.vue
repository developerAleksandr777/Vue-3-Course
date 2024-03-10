<template>
  <div class="loader__container">
    <span class="loader"></span>
  </div>
</template>

<script>
export default {
  name: "my-spinner",
};
</script>

<style scoped>
.loader__container {
  display: flex;
  align-items: center;
  justify-content: center;
  height: 100vh;
}
.loader {
  width: 48px;
  height: 48px;
  border: 5px solid teal;
  border-bottom-color: transparent;
  border-radius: 50%;
  display: inline-block;
  box-sizing: border-box;
  animation: rotation 1s linear infinite;
}

@keyframes rotation {
  0% {
    transform: rotate(0deg);
  }
  100% {
    transform: rotate(360deg);
  }
}
</style>
