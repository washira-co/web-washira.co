<template>
  <ol class="breadcrumb" itemscope itemtype="https://schema.org/BreadcrumbList">
    <li
      v-for="item in list"
      :key="item.position"
      itemprop="itemListElement"
      itemscope
      itemtype="https://schema.org/ListItem"
    >
      <a itemprop="item" :href="item.url">
        <span itemprop="name">{{ item.name }}</span>
      </a>
      <meta itemprop="position" :content="item.position" />
    </li>
  </ol>
</template>

<script lang="ts">
export default {
  props: ['list'],
}
</script>

<style lang="scss">
.breadcrumb {
  margin: 0;
  padding: 0;
  list-style: none;
}

.breadcrumb li {
  display: inline; /*横に並ぶように*/
  list-style: none;
  font-weight: bold; /*太字*/
}

.breadcrumb li:after {
  /* >を表示*/
  content: '>';
  padding: 0 0.2em;
  color: #555;
}

.breadcrumb li:last-child:after {
  content: '';
}

.breadcrumb li a {
  text-decoration: none;
  color: #52b5ee; /*色*/
}

.breadcrumb li a:hover {
  text-decoration: underline;
}
</style>
