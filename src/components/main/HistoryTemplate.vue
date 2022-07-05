<template>
  <section :id="history.id" class="mt-5">
    <h2>{{ history.title }}</h2>
    <div v-for="institution in history.timeline">
      <div class="text-end">{{ institution.duration }}</div>
      <h3 class="text-end m-0">{{ institution.name }}</h3>
      <div class="text-end">{{ institution.position }}</div>
      <p class="description my-4">{{ institution.description }}</p>
      <div v-for="project in institution.projects" class="mb-4">
        <strong>{{ project.name }}</strong><br>
        <em>{{ project.technologiesUsed }}</em>
        <p class="my-2">{{ project.description }}</p>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "HistoryTemplate",
  props: ["history"]
}
</script>
