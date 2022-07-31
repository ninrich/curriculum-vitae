<template>
  <HistoryTemplate
      :history="$data"
  />
</template>

<script>
import HistoryTemplate from "./HistoryTemplate.vue";

export default {
  name: "JobHistory",
  components: {HistoryTemplate},
  data() {
    return {
      id: "job-history",
      title: "Job history",
      timeline: [
        {
          name: "ESET, s.r.o.",
          duration: "2019 - 2020",
          position: "Junior Software Engineer",
          description:
              "In my 4th year of university, I was given an opportunity to go on a yearlong industrial placement. " +
              "What better place to start a career than the most successful Slovak IT company? What was initially " +
              "meant to be a summer internship got eventually extended for a whole year, and the only reason I left " +
              "ESET was to finish my education.",
          projects: [
            {
              name: "ESET Security Management Center",
              description:
                  "As a member of the Automation team I participated on various improvements of ESET's remote management " +
                  "tool currently known as ESET Protect. A backend developer from the start, I took on writing tests " +
                  "using the newly created API around halfway through my stay.",
              technologiesUsed: "C++, Python"
            }
          ]
        },
        {
          name: "hexamon.tech, s.r.o.",
          duration: "2020 - 2022",
          position: "Frontend developer",
          description:
              "During my last year of university I randomly met with a childhood friend and we decided to co-create " +
              "a (not only) car monitoring service. Almost ready to deploy the app to its first customers, we had to " +
              "put the project on hold due to lack of time on my friend's side caused by a once-in-a-lifetime opportunity.",
          projects: [
            {
              name: "Monbox",
              description:
                  "I develop the smartphone app which displays various data about customers' vehicles drawn from their " +
                  "OBD, such as their location, current speed, or trip history. With plans to add additional features, " +
                  "I also cooperate with a UX/UI designer and a backend developer on various screens and APIs.",
              technologiesUsed: "Framework7, Vue, Apache Cordova, GraphQL"
            },
          ]
        },
        {
          name: "Freelance",
          duration: "2022",
          position: "Web developer",
          description:
              "To meaningfully spend the time during Monbox hiatus by improving my frontend development skills, " +
              "I teamed up with a (not only graphic) designer friend to create some websites.",
          projects: [
            {
              name: "Invisible Parts",
              description:
                  "A local voluntary organization's effort aiming to map out and popularize various artworks in the " +
                  "public space in my hometown. Due to delays in other parts of project  the website development is " +
                  "currently put on hold.",
              technologiesUsed: "Vue"
            },
            {
              name: "Hory na Dosah",
              description:
                  "Helping an established mountain guide materialize his unique vision of how a perfect " +
                  "mountaineering experience should look like, we are collaboratively creating their brand identity " +
                  "and online presence.",
              technologiesUsed: "Vue"
            }
          ]
        }
      ]
    }
  }
}
</script>
