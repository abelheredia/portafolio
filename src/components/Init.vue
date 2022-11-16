<template>
  <div class="init">
    <div class="one">
      <div class="name">
        <h1>Abel Heredia</h1>
        <h3>Full Stack Developer</h3>
      </div>
    </div>
    <div class="two">
      <img src="@/assets/dev.png" alt="dev" />
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.init {
  width: 100%;
  height: calc(100vh - 4.5rem);
  display: flex;
}

.init .one {
  width: 50%;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
.init .one .name h1 {
  margin: 0;
}
.init .one .name h3 {
  color: #919191;
  margin: 0;
}

.init .two {
  width: 50%;
  background: #000;
  display: flex;
  justify-content: center;
  align-items: center;
}
.init .two img {
  width: 80%;
}

@media screen and (max-width: 768px) {
  .init {
    flex-direction: column-reverse;
  }

  .init .one {
    width: 100%;
    height: 40%;
  }
  .init .two {
    width: 100%;
    height: 60%;
  }
}
</style>
