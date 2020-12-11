<template>
  <section class="resume-section">
    <div class="resume-section-content">
      <h2 class="mb-5">
        {{ title }}
      </h2>
      <div v-for="edu in educations" :key="edu.id" class="d-flex flex-column flex-md-row justify-content-between mb-5">
        <div class="flex-grow-1">
          <h3 class="mb-0">
            {{ edu.degree }}
          </h3>
          <div class="subheading mb-3">
            <a :href="edu.school.website" :target="edu.school.website == '#' ? '_self' : '_blank'">
              {{ edu.school.name }}
            </a>
          </div>
          <ul>
            <li v-for="affiliation in edu.affliations" :key="affiliation.id">
              {{ affiliation.title }}
            </li>
          </ul>
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
          school: {
            name: 'Mindanao State University at Naawan',
            website: 'https://msunaawan.edu.ph'
          },
          degree: 'Bachelor of Science in Information Technology',
          affliations: [
            {
              id: 1,
              title: 'Majored in Database Management System'
            },
            {
              id: 2,
              title: 'Capstone Project: Student Information Management System for Lake View Academy in Don Carlos, Bukidnon'
            },
            {
              id: 3,
              title: 'Awarded Performing Arts in Music'
            },
            {
              id: 4,
              title: 'Member of Koro Kaayad Kaligaon Choir in Mindanao State University at Naawan'
            }
          ],
          duration: 'January 2016 - July 2020'
        },
        {
          id: 2,
          school: {
            name: 'Matangad National High School',
            website: '#'
          },
          degree: 'High School Diploma',
          affliations: [
            {
              id: 1,
              title: 'Graduated in Top 8 of Class'
            },
            {
              id: 2,
              title: 'Elected to Senator for Supreme Student Government in 2009'
            },
            {
              id: 3,
              title: 'Member of Supreme Student Government'
            }
          ],
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
