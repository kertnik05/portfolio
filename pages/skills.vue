<template>
  <section class="resume-section">
    <div class="resume-section-content">
      <h2 class="mb-5">
        {{ title }}
      </h2>
      <div class="subheading mb-3">
        Programming Languages &amp; Tools
      </div>
      <div class="row">
        <div class="col-sm">
          <div class="card" style="width: 18rem;">
            <div class="card-header bg-light">
              <h3 class="card-title text-center text-dark">
                <i class="fas fa-laptop-code" />
                Frontend
              </h3>
            </div>
            <div class="card-footer p-0">
              <ul class="nav flex-column">
                <li v-for="skill in skills" :key="skill.id" class="nav-item">
                  <a v-if="skill.category == 'frontend'" href="#" class="nav-link">
                    <i :class="skill.icon" />
                    {{ skill.tool }}
                  </a>
                  <div v-if="skill.category == 'frontend'" class="container">
                    <div class="progress mb-3" style="height: 10px;">
                      <div
                        class="progress-bar bg-info"
                        role="progressbar"
                        :style="{ width: skill.level + '%'}"
                      />
                    </div>
                  </div>
                </li>
              </ul>
            </div>
          </div>
        </div>
        <div class="col-sm">
          <div class="card" style="width: 18rem;">
            <div class="card-header bg-light">
              <h3 class="card-title text-center text-dark">
                <i class="fas fa-server" />
                Backend
              </h3>
            </div>
            <div class="card-footer p-0">
              <ul class="nav flex-column">
                <li v-for="skill in skills" :key="skill.id" class="nav-item">
                  <a v-if="skill.category == 'backend'" href="#" class="nav-link">
                    <i :class="skill.icon" />
                    {{ skill.tool }}
                  </a>
                  <div v-if="skill.category == 'backend'" class="container">
                    <div class="progress mb-3" style="height: 10px;">
                      <div
                        class="progress-bar bg-info"
                        role="progressbar"
                        :style="{ width: skill.level + '%'}"
                      />
                    </div>
                  </div>
                </li>
              </ul>
            </div>
          </div>
        </div>
        <div class="col-sm">
          <div class="card" style="width: 18rem;">
            <div class="card-header bg-light">
              <h3 class="card-title text-center text-dark">
                <i class="fas fa-tools" />
                Backend
              </h3>
            </div>
            <div class="card-footer p-0">
              <ul class="nav flex-column">
                <li v-for="skill in skills" :key="skill.id" class="nav-item">
                  <a v-if="skill.category == 'others'" href="#" class="nav-link">
                    <i :class="skill.icon" />
                    {{ skill.tool }}
                  </a>
                  <div v-if="skill.category == 'others'" class="container">
                    <div class="progress mb-3" style="height: 10px;">
                      <div
                        class="progress-bar bg-info"
                        role="progressbar"
                        :style="{ width: skill.level + '%'}"
                      />
                    </div>
                  </div>
                </li>
              </ul>
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
      title: 'Skills',
      skills: [
        {
          id: 1,
          tool: 'HTML',
          icon: 'fab fa-html5',
          level: 70,
          category: 'frontend'
        },
        {
          id: 2,
          tool: 'CSS',
          icon: 'fab fa-css3-alt',
          level: 50,
          category: 'frontend'
        },
        {
          id: 3,
          tool: 'JavaScript',
          icon: 'fab fa-js',
          level: 80,
          category: 'frontend'
        },
        {
          id: 4,
          tool: 'Vue.js',
          icon: 'fab fa-vuejs',
          level: 80,
          category: 'frontend'
        },
        {
          id: 5,
          tool: 'Bootstrap',
          icon: 'fab fa-bootstrap',
          level: 80,
          category: 'frontend'
        },
        {
          id: 6,
          tool: 'PHP',
          icon: 'fab fa-php',
          level: 80,
          category: 'backend'
        },
        {
          id: 7,
          tool: 'Laravel',
          icon: 'fab fa-laravel',
          level: 80,
          category: 'backend'
        },
        {
          id: 8,
          tool: 'MySQL',
          icon: 'fas fa-database',
          level: 70,
          category: 'backend'
        },
        {
          id: 9,
          tool: 'Java',
          icon: 'fab fa-java',
          level: 60,
          category: 'backend'
        },
        {
          id: 10,
          tool: 'Python',
          icon: 'fab fa-python',
          level: 50,
          category: 'backend'
        },
        {
          id: 11,
          tool: 'REST API',
          icon: 'fas fa-code',
          level: 80,
          category: 'others'
        },
        {
          id: 12,
          tool: 'GIT',
          icon: 'fab fa-git-alt',
          level: 80,
          category: 'others'
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

<style scoped>
a {
  text-decoration: none;
}
</style>
