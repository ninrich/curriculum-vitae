<template>
  <div class="pt-4">
    <AboutMe/>
    <EducationHistory/>
    <JobHistory/>
  </div>
</template>

<script>
import AboutMe from "./main/AboutMe.vue";
import EducationHistory from "./main/EducationHistory.vue";
import JobHistory from "./main/JobHistory.vue";
export default {
  name: "MainContent",
  components: {JobHistory, EducationHistory, AboutMe}
}
</script>
