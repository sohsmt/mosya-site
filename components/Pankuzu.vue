<template>
  <ol class="pankuzu">
    <li
      itemprop="itemListElement"
      itemscope
      itemtype="https://schema.org/ListItem"
    >
      <nuxt-link itemprop="item" to="/">
        <span itemprop="name">トップページ</span>
      </nuxt-link>
      <meta itemprop="position" content="1" />
    </li>
    <li
      itemprop="itemListElement"
      itemscope
      itemtype="https://schema.org/ListItem"
    >
      <span itemprop="name">{{ linkname }}</span>
      <meta itemprop="position" content="1" />
    </li>
  </ol>
</template>

<script>
export default {
  props: ['linkname'],
}
</script>
