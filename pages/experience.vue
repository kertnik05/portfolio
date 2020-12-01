<template>
  <section class="resume-section">
    <div class="resume-section-content">
      <h2 class="mb-5">
        {{ title }}
      </h2>
      <div v-for="exp in experiences" :key="exp.id" class="d-flex flex-column flex-md-row justify-content-between mb-5">
        <div class="flex-grow-1">
          <h3 class="mb-0">
            {{ exp.position }}
          </h3>
          <div class="subheading mb-3">
            {{ exp.company }}
          </div>
          <p>
            {{ exp.task }}
          </p>
        </div>
        <div class="flex-shrink-0">
          <span class="text-primary">
            {{ exp.duration }}
          </span>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data () {
    return {
      title: 'Experience',
      experiences: [
        {
          id: 1,
          position: 'Intern',
          company: 'Salusciens, Inc.',
          task: 'Conduct day-to-day software testing & bug reports',
          duration: 'January 2020 - March 2020'
        },
        {
          id: 2,
          position: 'Service Crew',
          company: 'Jollibee Gaisano',
          task: 'Dining Crew',
          duration: 'January 2015 - June 2015'
        }
      ]
    }
  },

  head () {
    return {
      title: `${this.title} | Nikko Lumahang`
    }
  }
}
</script>
