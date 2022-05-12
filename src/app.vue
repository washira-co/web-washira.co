<template>
  <Head>
    <!-- <Title>合同会社わしら</Title> -->
    <Link rel="icon" type="image/png" href="/img/logo/wasilogo03.png" />
    <!-- <Link rel="stylesheet" href="https://cdn.simplecss.org/simple.min.css" /> -->

    <Link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/css/bootstrap.min.css" />
    <Link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.3.1/css/all.css" />
    <Link rel="stylesheet" href="/template/free-hp.net/restaurant/re_001/css/style.css" />
    <Link rel="stylesheet" href="/css/template_customize.css" />
  </Head>

  <TheHeaderMenu />

  <main>
    <NuxtPage />
  </main>

  <TheFooterMenu />

  <!-- javascript はここから -->
  <Script type="text/javascript" src="https://code.jquery.com/jquery-3.3.1.slim.min.js" />
  <Script type="text/javascript" src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.3/umd/popper.min.js" />
  <Script type="text/javascript" src="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/js/bootstrap.min.js" />
  <Script type="text/javascript" src="/template/free-hp.net/restaurant/re_001/js/script.js" />
</template>

<script setup>
const route = useRoute()

useHead({
  title: computed(() => `${route.meta.title} | 合同会社わしら`),
})
</script>

<style lang="scss" scoped></style>
