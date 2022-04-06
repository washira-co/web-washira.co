<template>
  <Head>
    <!-- <Title>合同会社わしら</Title> -->
    <Link rel="icon" type="image/png" href="/img/logo/wasilogo03.png" />
    <Link rel="stylesheet" href="https://cdn.simplecss.org/simple.min.css" />
  </Head>

  <div>
    <NuxtPage />
  </div>
</template>

<script setup>
const route = useRoute();

useHead({
  title: computed(() => `${route.meta.title} | 合同会社わしら`),
});
</script>

<style lang="scss" scoped></style>
