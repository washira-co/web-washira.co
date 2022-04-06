<template>
  <Head>
    <!-- <Title>合同会社わしら</Title> -->
    <Link rel="icon" type="image/png" href="/img/logo/wasilogo03.png" />
    <Link rel="stylesheet" href="https://cdn.simplecss.org/simple.min.css" />
    <!-- Clarity tracking code for https://washira.co/ -->
    <!-- <Script>
      (function(c,l,a,r,i,t,y){
      c[a]=c[a]||function(){(c[a].q=c[a].q||[]).push(arguments)};
      t=l.createElement(r);t.async=1;t.src="https://www.clarity.ms/tag/"+i+"?ref=bwt";
      y=l.getElementsByTagName(r)[0];y.parentNode.insertBefore(t,y);
      console.log("てすとーーーーーーーーーー"); })(window, document, "clarity", "script",
      "bco2d1bfoy");
    </Script> -->
    <Script> console.log("てすとーーーーーーーーーー"); </Script>
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
