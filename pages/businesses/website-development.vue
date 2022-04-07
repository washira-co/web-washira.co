<template>
  <div>
    <BreadcrumbList :list="breadcrumbList" />
  </div>

  <div>
    <h2>WEBサイト制作/運用</h2>
    <h3>作るから運用し、成果を目指すWEBサイト制作</h3>
    <p>
      なぜ、WEBサイトを持つのか、持ったあとどう運用していくのか?
      きちんと成果は出ているのか?<br />
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
    ></iframe>
  </div>

  <div>
    <h3>お問い合わせ</h3>
    <a
      href="https://tayori.com/form/c787ef402de80671fcd7ddb66d6e27d987bb8210/"
      target="_blank"
    >
      <button>お問い合わせはこちら</button>
    </a>
  </div>
</template>

<script lang="ts">
export default {
  async setup() {
    definePageMeta({
      title: "WEBサイト制作/運用",
    });

    /** パンくず */
    const breadcrumbList = [
      {
        name: "トップ",
        url: "/",
        position: "1",
      },
      {
        name: "事業内容",
        url: "/businesses/",
        position: "2",
      },
      {
        name: "WEBサイト制作/運用",
        url: "/businesses/website-development/",
        position: "3",
      },
    ];

    return {
      breadcrumbList,
    };
  },
};
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
