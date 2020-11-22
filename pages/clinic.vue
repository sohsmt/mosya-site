<template>
  <div class="clinic">
    <Pankuzu linkname="医院紹介" />
    <div class="clinic_main">
      <Sidemenu />
      <div class="main-contents_wrapper">
        <h2>医院紹介</h2>
        <div class="main-contents"></div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      linkname: '',
    }
  },
}
</script>
