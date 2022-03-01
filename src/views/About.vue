<template>
  <div>
    <div class="about">
      <div class="logo">
        <router-link to="/">
          <img src="../assets/sisterwiveslogo.png" alt=""
        /></router-link>
      </div>
      <div class="text">
        <p class="top">We recycle and reuse things to adorn ourselves.</p>
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

.top {
  margin-top: 0;
}

p {
  margin: 2rem 0;
}

@media only screen and (max-width: 750px) {
  .logo {
    display: block;
  }
}
</style>
