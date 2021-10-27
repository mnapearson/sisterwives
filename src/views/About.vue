<template>
  <div>
    <div class="about">
      <div class="text">
        <p>We recycle and reuse things to adorn ourselves.</p>
        <p>We design and build websites.</p>
        <p>We curate art and music.</p>
        <p>We make magic.</p>
      </div>
    </div>
  </div>
</template>

<style scoped>
@font-face {
  font-family: "Metana-bold";
  src: url(../fonts/NeueMetana-Bold.otf);
}

.about {
  -webkit-animation: fade-in 1.75s cubic-bezier(0.39, 0.575, 0.565, 1) both;
  animation: fade-in 1.75s cubic-bezier(0.39, 0.575, 0.565, 1) both;
}

.text {
  margin: 2rem;
}

p {
  margin: 3rem 0;
}
</style>
