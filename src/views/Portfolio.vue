<template>
  <div>
    <div class="portfolio">
      <div class="sites">
        <a
          target="_blank"
          rel="noopener noreferrer"
          href="https://ispyleipzig.netlify.app"
        >
          <h1 class="link">i spy</h1></a
        >
        <a
          target="_blank"
          rel="noopener noreferrer"
          href="https://devhausleipzig.de"
        >
          <h1 class="link">devhaus</h1></a
        >
        <a
          target="_blank"
          rel="noopener noreferrer"
          href="http://henrikbaumgarten.com/"
        >
          <h1 class="link">traumgaben</h1></a
        >
        <a
          target="_blank"
          rel="noopener noreferrer"
          href="https://celestial-weather.netlify.app/"
        >
          <h1 class="link">celestial</h1></a
        >
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Portfolio",
};
</script>

<style scoped>
.sites {
  display: flex;
  flex-direction: column;
  -webkit-animation: fade-in 1.75s cubic-bezier(0.39, 0.575, 0.565, 1) both;
  animation: fade-in 1.75s cubic-bezier(0.39, 0.575, 0.565, 1) both;
}

a {
  text-decoration: none;
}

.link {
  margin-top: 3rem;
}
</style>
