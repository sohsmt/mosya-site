<template>
  <footer class="footer">
    <div class="footer_menu">
      <ul>
        <li v-for="item in items" :key="item">
          <a href="#">{{ item }}</a>
        </li>
        <!-- <li>
          <a href="#">トップページ</a>
        </li>
        <li>
          <a href="#">医院紹介</a>
        </li>
        <li>
          <a href="#">診療紹介</a>
        </li>
        <li>
          <a href="#">院長・スタッフ紹介</a>
        </li>
        <li>
          <a href="#">アクセス</a>
        </li> -->
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
      items: [
        'トップページ',
        '医院紹介',
        '診療紹介',
        '院長・スタッフ紹介',
        'アクセス',
        // { menu: 'トップページ' },
        // { menu: '医院紹介' },
        // { menu: '診療紹介' },
        // { menu: '院長・スタッフ紹介' },
        // { menu: 'アクセス' },
      ],
    }
  },
}
</script>
