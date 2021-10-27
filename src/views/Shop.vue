<template>
  <div classs="shop">
    <h1>coming soon</h1>
  </div>
</template>

<script>
export default {
  name: "Shop",
};
</script>

<style scoped>
h1 {
  -webkit-animation: blink-1 10s infinite both;
  animation: blink-1 10s infinite both;
}

@-webkit-keyframes blink-1 {
  0%,
  50%,
  100% {
    opacity: 1;
  }
  25%,
  75% {
    opacity: 0;
  }
}
@keyframes blink-1 {
  0%,
  50%,
  100% {
    opacity: 1;
  }
  25%,
  75% {
    opacity: 0;
  }
}
</style>
