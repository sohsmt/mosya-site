<template>
  <footer class="footer">
    <div class="footer_menu">
      <ul>
        <li v-for="link in links" :key="link">
          <nuxt-link :to="link.path">{{ link.label }}</nuxt-link>
        </li>
      </ul>
    </div>
    <div class="footer_address">
      <p>
        <span>デンタル クリニック</span> 東京都新宿区市谷左内町21-13
        TEL:03-0000-0000
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
    return {
      links: [
        { label: 'トップぺージ', span: 'HOME', path: '/' },
        { label: '医院紹介', span: 'CLINIC', path: '/clinic' },
        { label: '診療案内', span: 'SERVICE', path: '/service' },
        { label: '院長・スタッフ紹介', span: 'STAFF', path: '/staff' },
        { label: 'アクセス', span: 'ACCESS', path: '/access' },
      ],
    }
  },
}
</script>
