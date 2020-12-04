<template>
  <section class="resume-section">
    <div class="resume-section-content">
      <h2 class="mb-5">
        {{ title }}
      </h2>
      <div class="row">
        <div v-for="project in projects" :key="project.id" class="col-sm">
          <div class="card mb-3" style="width: 19rem;">
            <div class="card-header bg-light">
              <h3 class="card-title text-center text-dark">
                <a :href="project.github_link" target="_blank">
                  {{ project.title }}
                </a>
              </h3>
            </div>
            <div class="card-body">
              {{ project.description }}
            </div>
            <div class="card-footer">
              <span v-for="tool in project.tools" :key="tool" class="badge badge-info mr-2">
                {{ tool }}
              </span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data () {
    return {
      title: 'Projects',
      projects: [
        {
          id: 1,
          title: 'LVA',
          description: 'Undergrad Capstone Project Student Information Management System for Lake View Academy in Don Carlos, Bukidnon built in Laravel Framework & Vue.js',
          github_link: 'https://github.com/kertnik05/LVA',
          tools: ['PHP', 'HTML', 'CSS', 'JavaScript', 'Laravel', 'Vue.js']
        },
        {
          id: 2,
          title: 'e-commerce',
          description: 'Ecommerce app built with Laravel & Vue.js',
          github_link: 'https://github.com/kertnik05/e-commerce',
          tools: ['PHP', 'HTML', 'CSS', 'JavaScript', 'Laravel', 'Vue.js']
        },
        {
          id: 3,
          title: 'vue-boilerplate',
          description: 'Vue.js 3 Single File Component Biolerplate using Laravel Mix',
          github_link: 'https://github.com/kertnik05/vue-boilerplate',
          tools: ['HTML', 'CSS', 'JavaScript', 'Vue.js', 'Laravel Mix']
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
