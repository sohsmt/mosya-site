<template>
  <div class="header">
    <div class="site__top">
      <div class="site__title">
        <img src="~/assets/image/siteTitle.png" alt="サイトタイトル" />
      </div>
      <div class="site__info">
        <p>"地域に根付いた歯科医院"デンタルクリニック</p>
        <p class="site__info-2">03-0000-0000</p>
        <div class="site__info-time">
          <p>予約受付時間 10:00～19:30 <span>日祝 休診</span></p>
        </div>
      </div>
    </div>
    <div class="site__nav">
      <nav class="nav">
        <ul>
          <li v-for="link in links" :key="link.label">
            <nuxt-link :to="link.path">
              <P
                >{{ link.label }} <br /><span>{{ link.span }}</span>
              </P>
            </nuxt-link>
          </li>
        </ul>
      </nav>
    </div>
    <p>{{ test }}</p>
  </div>
</template>

<style lang="scss"></style>

<script>
export default {
  data() {
    return {}
  },
  computed: {
    links() {
      return this.$store.state.links.links
    },
  },
}
</script>
