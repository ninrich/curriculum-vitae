<template>
  <HistoryTemplate
    :history="$data"
  />
</template>

<script>
import HistoryTemplate from "./HistoryTemplate.vue";
export default {
  name: "EducationHistory",
  components: {HistoryTemplate},
  data() {
    return {
      id: "education-history",
      title: "Education",
      timeline: [
        {
          name: "University of Aberdeen",
          duration: "2016 - 2021",
          position: "Master in Computing Science",
          description:
              "After finishing high school, I had to leave my hometown to pursue higher education. So why not " +
              "choose a different country altogether? Split between psychology and computing science, " +
              "I chose the latter in Year 2 and finished with Upper Second Class Honours.",
          projects: [
            {
              name: "IoT System for Monitoring Household Electric Energy Consumption",
              description:
                  "For my dissertation I created a tool which clamps onto a consumer unit and measures electrical " +
                  "current flowing through the live wire. The tool then wirelessly sends measured data onto a web " +
                  "server, which allows the user to view various statistics and graphs detailing their electricity " +
                  "usage.",
              technologiesUsed: "Arduino, C++, Raspberry Pi, Python"
            }
          ]
        }
      ]
    }
  }
}
</script>
