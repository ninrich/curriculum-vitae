<template>
  <section id="skills" class="my-4 px-1">
    <div v-for="(level, skill) in $data" :key="skill" class="row">
      <div class="col-6 justify-content-start">
        <label for="progress-placeholder">{{ skill }}</label>
      </div>
      <div class="col-6 justify-content-end">
        <progress id="progress-placeholder" :value="level" max="100"> {{ level }}% </progress>
      </div>
    </div>
  </section>
</template>


<script>
export default {
  name: "SkillsWidget",
  data() {
    return {
      "HTML" : 80,
      "CSS" : 80,
      "Vue" : 75,
      "JavaScript": 72,
      "Python" : 69,
      "C++" : 60,
    }
  },
}
</script>

<style lang="scss" scoped>
@import "@/scss/custom";

label {
  font-weight: 600;
}

progress {
  border: 0.2rem solid $primary;
  border-radius: 3px;
  width: 100%;
  height: 1.5rem;
}

progress::-webkit-progress-bar {
  background-color: transparent;
}

progress::-webkit-progress-value {
  background-color: $primary;
}

progress::-moz-progress-bar {
  background-color: transparent;
}
</style>
