<template>
  <nav aria-label="breadcrumb" class="breadcrumb">
    <ol class="breadcrumb container py-0 mb-0" itemscope itemtype="https://schema.org/BreadcrumbList">
      <!-- <li class="breadcrumb-item"><a href="../index.html">ホーム</a></li> -->
      <!-- <li class="breadcrumb-item active">お問い合わせ</li> -->
      <li
        v-for="item in list"
        :key="item.position"
        itemprop="itemListElement"
        itemscope
        itemtype="https://schema.org/ListItem"
        :class="`${item.active ? 'active ' : ''}breadcrumb-item`"
      >
        <a itemprop="item" :href="item.url">
          <span itemprop="name">{{ item.name }}</span>
        </a>
        <meta itemprop="position" :content="item.position" />
      </li>
    </ol>
  </nav>
</template>

<script lang="ts">
export default {
  props: {
    list: {
      type: Array,
      required: true,
    },
  },
}
</script>

<style lang="scss"></style>
