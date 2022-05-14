<template>
  <BreadcrumbList :list="breadcrumbList" />

  <section id="section-businesses" class="py-5 container">
    <h2 class="font-weight-bold text-center ttl-bdr">WEBサイト制作/運用</h2>
    <div class="row py-4 justify-content-center">
      <h3 class="h2 font-weight-bold">設計→制作→運用/カイゼンへ、成果を目指すWEBサイト制作</h3>

      <div class="col-md-10 text-center">
        <div class="lead text-left">
          <p>
            なぜ、WEBサイトを持つのか、持ったあとどう運用していくのか? きちんと成果は出ているのか?<br />
            作るから成果が出るまでを、「内製チーム」のように進めていきます。<br />
            製作は、請負契約でコスト感や納期感にあわせて制作/リリースを行います。<br />
            リリース後は、準委任契約で、サイトの運用/カイゼンや効果測定などサポートさせて頂くことも可能です。<br />
            最新の技術トレンドを追っていますので、今最適な構成で設計/作成しています。<br />
            見た目だけに終わらない、成果の出るサイトを一緒に作りましょう。
          </p>
        </div>

        <div class="iframe-outer">
          <iframe
            class="iframe-tags"
            src="https://docs.google.com/presentation/d/e/2PACX-1vQuDXWi8kFIuTT1PLwvExsOVYD8bwmePxwZboaoepewYjGcqQmqlj0Lk2fym3iVfwD5tuMud3atJk-S/embed?start=false&loop=false&delayms=60000"
            frameborder="0"
            width="960"
            height="569"
            allowfullscreen="true"
            mozallowfullscreen="true"
            webkitallowfullscreen="true"
          />
        </div>
        <div class="text-center">
          <a
            class="btn font-weight-bold"
            href="https://tayori.com/form/c787ef402de80671fcd7ddb66d6e27d987bb8210/"
            target="_blank"
            role="button"
            >お問い合わせ</a
          >
        </div>
      </div>
    </div>
  </section>
</template>

<script lang="ts">
export default {
  setup() {
    definePageMeta({
      title: 'WEBサイト制作/運用',
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
        active: false,
      },
      {
        name: 'WEBサイト制作/運用',
        url: '/businesses/website-development/',
        position: '3',
        active: true,
      },
    ]

    return {
      breadcrumbList,
    }
  },
}
</script>

<style lang="scss">
.iframe-outer {
  position: relative;
  padding-top: 75%; /*4:3の縦横比率にしたい場合、3÷4=75%*/
}

.iframe-tags {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
}
</style>
