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
          <ul>
            <li v-for="task in exp.tasks" :key="task.id">
              {{ task.name }}
            </li>
          </ul>
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
          position: 'Student Intern',
          company: 'Salusciens, Inc.',
          tasks: [
            {
              id: 1,
              name: 'Collaborated with product managers, testers, and developers to initiate process improvements.'
            },
            {
              id: 2,
              name: 'Collaborated with project managers, testers, end-users, and distributors.'
            }
          ],
          duration: 'January 2020 - March 2020'
        },
        {
          id: 2,
          position: 'Service Crew',
          company: 'Jollibee Gaisano',
          tasks: [
            {
              id: 1,
              name: 'Carried out complete opening, closing and shift change duties to keep restaurant working efficiently and teams ready to meet customer needs.'
            },
            {
              id: 2,
              name: 'Maintained customer satisfaction with timely table check-ins to assess food and beverage needs.'
            },
            {
              id: 3,
              name: 'Kept server areas clean and stocked during service hours to increase efficiency while working tables.'
            },
            {
              id: 4,
              name: 'Decreased customer wait times by enlisting coworkers assistance for multi-order delivery to avoid spilling or dropping food.'
            },
            {
              id: 5,
              name: 'Monitored dining rooms for seating availability as well as service, safety and well-being of guests.'
            },
            {
              id: 6,
              name: 'Maintained order efficiency and accuracy through clear communication with kitchen staff, earning numerous recommendations from satisfied customers.'
            },
            {
              id: 7,
              name: 'Collaborated with kitchen staff to correctly update customers on unavailable dishes and wait times.'
            }
          ],
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
