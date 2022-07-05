<template>
  <section id="personal-info">
    <div class="row justify-content-center">
      <div class="col-8 col-md-12 my-4 px-4">
        <img alt="Imagine Brad Pitt, but younger." src="/assets/me.jpeg">
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "PersonalInfo"
}
</script>

<style lang="scss" scoped>
@import "@/scss/custom";

img {
  max-width: 100%;
  border-radius: 50%;
  border: 0.5em solid $primary;
}
</style>
