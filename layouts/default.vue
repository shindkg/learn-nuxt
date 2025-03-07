<template>
  <div>
    <!-- route -->
    <h1>{{ $route.name }} (default.vue 라우트) 페이지</h1>
    <!-- NuxtLink == router-link -->
    <NuxtLink to="/">홈페이지</NuxtLink>
    <NuxtLink to="/main">메인페이지</NuxtLink>
    <NuxtLink to="/product">상품페이지</NuxtLink>
    <!-- Nuxt == router-view -->
    <Nuxt />
  </div>
</template>

<script>
export default {
  created() {
    console.log(this.$route)
  }
}
</script>
