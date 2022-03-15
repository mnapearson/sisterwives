<template>
  <div>
    <div class="portfolio">
      <div class="sites">
        <router-link to="ispy"> <h1 class="link">i spy</h1></router-link>

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
        ><a
          target="_blank"
          rel="noopener noreferrer"
          href="https://antarkeith.com/"
        >
          <h1 class="link">antar keith</h1></a
        >
        <a
          target="_blank"
          rel="noopener noreferrer"
          href="https://wellroundedhoodlum.com/"
        >
          <h1 class="link">hendershot</h1></a
        >
        <a
          target="_blank"
          rel="noopener noreferrer"
          href="https://beenseen.netlify.app/"
        >
          <h1 class="link">been seen</h1></a
        ><a
          target="_blank"
          rel="noopener noreferrer"
          href="https://zencal-b5217.web.app/"
        >
          <h1 class="link">zencal</h1></a
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
.link {
  margin-top: 2rem;
}

.portfolio {
  margin-top: 3rem;
}
</style>
