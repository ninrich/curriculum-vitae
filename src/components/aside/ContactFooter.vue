<template>
  <footer>
    <div class="row px-4 py-2">
      <div v-for="(url, platform) in $data" class="col text-center">
        <a :href="url" class="contact">
          <img :src="`/assets/icons/${platform}.svg`" :alt="`${platform} icon`"/>
        </a>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "ContactFooter",
  data() {
    return {
      "email": "mailto:nino.trnovsky@gmail.com",
      "linkedin": "https://www.linkedin.com/in/ninrich/",
      "github": "https://github.com/ninrich/curriculum-vitae"
    }
  }
}
</script>

<style lang="scss" scoped>
@import "@/scss/custom.scss";

footer {
  margin-top: auto;
  border-top: 0.2rem solid $primary;
}

.contact {
  border: none;
  background-color: transparent;
  text-align: center;
}

.contact > img {
  max-height: 2rem;
  max-width: 2rem;
}
</style>
