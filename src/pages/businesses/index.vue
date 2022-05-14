<template>
  <BreadcrumbList :list="breadcrumbList" />

  <section id="section-businesses" class="py-5 container">
    <h2 class="font-weight-bold text-center ttl-bdr">事業内容</h2>
    <div class="row py-4 justify-content-center">
      <div class="col-md-6 text-center">
        <div class="lead text-left">
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
      </div>
    </div>
  </section>
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
        active: false,
      },
      {
        name: '事業内容',
        url: '/businesses/',
        position: '2',
        active: true,
      },
    ]

    return {
      breadcrumbList,
    }
  },
}
</script>
