<template>
  <header class="pt-4">
    <h1 class="display-1 text-uppercase text-center m-0">
      An&shy;ton<br>Tr&shy;nov&shy;ský
    </h1>
  </header>
</template>

<script>
export default {
  name: "PageHeader"
}
</script>

<style lang="scss">
@import "@/scss/custom.scss";

@include media-breakpoint-up(md) {
  .display-1 {
    font-size: 2.5rem !important;
  }
}
</style>