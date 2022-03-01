<template>
  <div class="episodes">
    <div>
      <iframe
        style="border-radius: 12px"
        src="https://open.spotify.com/embed/playlist/0ZBLSZ7sSWQBRYqtmUsOEV?utm_source=generator"
        width="100%"
        height="380"
        frameBorder="0"
        allowfullscreen=""
        allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture"
      ></iframe>
    </div>
    <p>scroll for more...</p>
    <div class="episode">
      <iframe
        style="border-radius: 12px"
        src="https://open.spotify.com/embed/playlist/0sk5DDihMEZpp1fU0hQJC8?utm_source=generator"
        width="100%"
        height="380"
        frameBorder="0"
        allowfullscreen=""
        allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture"
      ></iframe>
    </div>
    <div class="episode">
      <iframe
        style="border-radius: 12px"
        src="https://open.spotify.com/embed/playlist/7Ek67HMX0wlQUjGZJyXIRZ?utm_source=generator"
        width="100%"
        height="380"
        frameBorder="0"
        allowfullscreen=""
        allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture"
      ></iframe>
    </div>
    <div class="episode">
      <iframe
        style="border-radius: 12px"
        src="https://open.spotify.com/embed/playlist/05aOxVSYdgmmDXLcNT1juo?utm_source=generator"
        width="100%"
        height="380"
        frameBorder="0"
        allowfullscreen=""
        allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture"
      ></iframe>
    </div>
    <div class="episode">
      <iframe
        style="border-radius: 12px"
        src="https://open.spotify.com/embed/playlist/0Qhkh1BuRZOpRyS1LGbh8p?utm_source=generator"
        width="100%"
        height="380"
        frameBorder="0"
        allowfullscreen=""
        allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture"
      ></iframe>
    </div>
    <div class="episode">
      <iframe
        style="border-radius: 12px"
        src="https://open.spotify.com/embed/playlist/13LLDWMNKCZ0v5ORLeTxHv?utm_source=generator"
        width="100%"
        height="380"
        frameBorder="0"
        allowfullscreen=""
        allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture"
      ></iframe>
    </div>
  </div>
</template>

<script>
export default {
  name: "Radio",
};
</script>

<style scoped>
.episodes {
  display: flex;
  flex-direction: column;
  height: 450px;
  width: 350px;
  margin: 2rem;
  overflow-y: scroll;
}

.episode {
  margin-top: 2rem;
}
</style>
