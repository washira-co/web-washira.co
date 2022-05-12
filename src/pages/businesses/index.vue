<template>
  <div>
    <BreadcrumbList :list="breadcrumbList" />
  </div>

  <div>
    <h2>事業内容 <small>[Businesses]</small></h2>
    <ul>
      <li>猫を幸せにする事業</li>
      <li>
        IT部門委託事業
        <ul>
          <li>
            <a href="https://techmesse.com/tech/1278" target="_blank"
              >情報システム部門チームのアウトソーシング | TechMesse</a
            >
          </li>
        </ul>
      </li>
      <li>IT部門内製化支援事業</li>
      <li>
        <a href="/businesses/website-development/">WEBサイト制作/運用</a>
      </li>
    </ul>
  </div>
</template>

<script lang="ts">
export default {
  setup() {
    definePageMeta({
      title: '事業内容',
    })

    /** パンくず */
    const breadcrumbList = [
      {
        name: 'トップ',
        url: '/',
        position: '1',
      },
      {
        name: '事業内容',
        url: '/businesses/',
        position: '2',
      },
    ]

    return {
      breadcrumbList,
    }
  },
}
</script>
