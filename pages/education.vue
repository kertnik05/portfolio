<template>
  <section class="resume-section">
    <div class="resume-section-content">
      <h2 class="mb-5">
        {{ title }}
      </h2>
      <div v-for="edu in educations" :key="edu.id" class="d-flex flex-column flex-md-row justify-content-between mb-5">
        <div class="flex-grow-1">
          <h3 class="mb-0">
            {{ edu.school }}
          </h3>
          <div class="subheading mb-3">
            {{ edu.degree }}
          </div>
          <div>
            {{ edu.course }} - {{ edu.major }}
          </div>
        </div>
        <div class="flex-shrink-0">
          <span class="text-primary">
            {{ edu.duration }}
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
      title: 'Education',
      educations: [
        {
          id: 1,
          school: 'Mindanao State University at Naawan',
          degree: 'Bachelor of Science',
          course: 'Information Technology',
          major: 'Database Management System',
          duration: 'January 2016 - July 2020'
        },
        {
          id: 2,
          school: 'Matangad National High School',
          degree: 'High School Diploma',
          course: '',
          major: '',
          duration: 'January 2016 - July 2020'
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
