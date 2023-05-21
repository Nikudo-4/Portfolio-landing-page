<template>
  <div class="container">
    <b-nav class="justify-content-between">
      <b-nav-item active>
        <nuxt-link to="/">{{ $t("home") }}</nuxt-link>
      </b-nav-item>
      <b-nav-item><nuxt-link to="/about">{{ $t("about") }}</nuxt-link></b-nav-item>
      <b-nav-item><nuxt-link to="/about">{{ $t("skills") }}</nuxt-link></b-nav-item>
      <b-nav-item><nuxt-link to="/about">{{ $t("portfolio") }}</nuxt-link></b-nav-item>
      <b-nav-item><nuxt-link to="/about">{{ $t("contacts") }}</nuxt-link></b-nav-item>
    </b-nav>
    <section class="name">
      <div class="container">
        <div class="row justify-content-between">
          <div class="name">
            <div class="name__name">{{ $t("name") }}</div>
            <div class="name__surname">{{ $t("surname") }}</div>
          </div>
          <div class="row">
            <nuxt-link :to="localePath('index', 'ru')">Homepage in English</nuxt-link>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  name: "IndexPage",
  data() {
    return {

      }
    },
    methods: {
      changeLocal() {
      // console.log("33312333")

    },

    },
};
</script>

<style  scoped>

.nav li:first-child a{
padding-left: 0;
}
.nav li:last-child a{
padding-right: 0;
}
</style>