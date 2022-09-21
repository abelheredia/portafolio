<template>
  <div class="foot">
    <div class="logos">
      <img
        src="../assets/facebook.svg"
        alt="facebook"
        @click="openLink('https://www.facebook.com/abel.herediabravo')"
      />
      <img
        src="../assets/linkedin.svg"
        alt="linkedin"
        @click="openLink('https://www.linkedin.com/in/abelheredia/')"
      />
      <img
        src="../assets/instagram.svg"
        alt="instagram"
        @click="openLink('https://www.instagram.com/abelherediabravo/')"
      />
    </div>
    <h3>Abel Heredia Bravo</h3>
  </div>
</template>

<script>
export default {
  methods: {
    openLink(link) {
      window.open(link);
    },
  },
};
</script>

<style scoped>
.foot {
  background-color: #000;
  width: 100%;
  height: 15rem;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  color: #fff;
}

.logos img {
  margin: 0 0.5rem;
  cursor: pointer;
}

h3 {
  font-size: 18px;
}
</style>
