<template>
  <footer class="footer">
    <div class="footer_menu">
      <ul>
        <li v-for="link in links" :key="link.index">
          <nuxt-link :to="link.path">{{ link.label }}</nuxt-link>
        </li>
      </ul>
    </div>
    <div class="footer_address">
      <p>
        <span class="address_bold">デンタル クリニック</span>
        <span>東京都新宿区市谷左内町21-13</span>
        <span>TEL:03-0000-0000</span>
      </p>
    </div>
    <div class="footer_coppyright">
      <small>Copyright 2012 Dental Clinic CO.,LTD All Rights Reserved.</small>
    </div>
  </footer>
</template>

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
