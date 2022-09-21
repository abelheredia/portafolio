<template>
  <div class="skills">
    <div class="title">
      <h2>SKILLS</h2>
    </div>
    <div class="logos">
      <div v-for="logo in logos" :key="logos.indexOf(logo)">
        <img :src="logo.url" height="100" width="106" />
        <h4>{{ logo.name }}</h4>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Habilidades",
  data: function () {
    return {
      logos: [
        { name: "JAVASCRIPT", url: require("@/assets/javascript.svg") },
        { name: "PYTHON", url: require("@/assets/python.svg") },
        { name: "ANGULAR", url: require("@/assets/angular.svg") },
        { name: "REACT", url: require("@/assets/react.svg") },
        { name: "VUE", url: require("@/assets/vue.svg") },
        { name: "HTML", url: require("@/assets/html.svg") },
        { name: "CSS", url: require("@/assets/css.svg") },
        { name: "GOLANG", url: require("@/assets/golang.svg") },
        { name: "NODE", url: require("@/assets/node.svg") },
        { name: "MYSQL", url: require("@/assets/mysql.svg") },
        { name: "ORACLE", url: require("@/assets/oracle.svg") },
        { name: "SQL", url: require("@/assets/sql-server.svg") },
        { name: "AWS", url: require("@/assets/aws.svg") },
        { name: "FLUTTER", url: require("@/assets/flutter.svg") },
        { name: "PHP", url: require("@/assets/php.svg") },
        { name: "LARAVEL", url: require("@/assets/laravel.svg") },
      ],
    };
  },
};
</script>

<style scoped>
.skills {
  padding: 2rem 0;
}

.skills .title {
  width: 12rem;
  border: 8px solid #000000;
  margin: 0 auto;
}

.skills .logos {
  margin: 3rem auto 0 auto;
  width: 60%;
  display: grid;
  grid-template-columns: 25% 25% 25% 25%;
  row-gap: 2rem;
}

.skills .logos img {
  margin: 0 auto;
}

@media screen and (max-width: 768px) {
  .skills .logos {
    width: 100%;
    grid-template-columns: 50% 50%;
  }
}
</style>
