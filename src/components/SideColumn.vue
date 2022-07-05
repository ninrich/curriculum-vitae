<template>
  <div class="side-column-container px-2 px-md-0">
    <!-- <header> is intentionally not in <aside>
       https://stackoverflow.com/a/6109160  -->
    <PageHeader/>
    <aside>
      <PersonalInfo/>
      <SkillsWidget/>
    </aside>
    <ContactFooter/>
  </div>
</template>
<script>
import PersonalInfo from "../components/aside/PersonalInfo.vue"
import PageHeader from "../components/aside/PageHeader.vue";
import SkillsWidget from "../components/aside/SkillsWidget.vue";
import ContactFooter from "./aside/ContactFooter.vue";

export default {
  name: 'SideColumn',
  components: {ContactFooter, SkillsWidget, PageHeader, PersonalInfo}
}
</script>

<style>
.side-column-container {
  display: flex;
  flex-direction: column;
  min-height: 100%;
}
</style>
