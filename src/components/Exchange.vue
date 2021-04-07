<template>
  <div id="exchange">
    <div class="wrapper">
      Bursa
    </div>
  </div>
</template>

<script>
export default {
  name: 'Exchange'
}
</script>

<style scoped>
.wrapper {
  height: 40px;
  width: 64px;
  background-color: yellow;
  text-align: center;
  justify-content: center;
  transform-origin: center;
  transform: rotate(-90deg);

  /* Legacy vendor prefixes that you probably don't need... */

  /* Safari */
  -webkit-transform: rotate(270deg);

  /* Firefox */
  -moz-transform: rotate(270deg);

  /* IE */
  -ms-transform: rotate(270deg);

  /* Opera */
  -o-transform: rotate(270deg);

  /* Internet Explorer */
  filter: progid:DXImageTransform.Microsoft.BasicImage(rotation=3);
}
</style>
