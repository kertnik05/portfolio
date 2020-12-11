<template>
  <nav id="sideNav" class="navbar navbar-expand-lg navbar-dark bg-primary fixed-top">
    <nuxt-link class="navbar-brand js-scroll-trigger" to="/">
      <span class="d-block d-lg-none">
        Kert Rey Nikko Lumahang
      </span>
      <span class="d-none d-lg-block">
        <img class="img-fluid img-profile rounded-circle mx-auto mb-2" src="~/assets/img/profile2.jpeg" alt="profile">
      </span>
    </nuxt-link>
    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent">
      <span class="navbar-toggler-icon" />
    </button>
    <div id="navbarSupportedContent" class="collapse navbar-collapse">
      <ul class="navbar-nav">
        <li v-for="route in routes" :key="route.id" class="nav-item">
          <nuxt-link class="nav-link" :to="route.link">
            {{ route.name }}
          </nuxt-link>
        </li>
      </ul>
    </div>
  </nav>
</template>

<script>
export default {
  data () {
    return {
      routes: [
        {
          id: 1,
          name: 'About',
          link: '/about'
        },
        {
          id: 2,
          name: 'Experience',
          link: '/experience'
        },
        {
          id: 3,
          name: 'Education',
          link: '/education'
        },
        {
          id: 4,
          name: 'Skills',
          link: '/skills'
        },
        {
          id: 4,
          name: 'Interests',
          link: '/interests'
        },
        {
          id: 5,
          name: 'Projects',
          link: '/projects'
        }
      ]
    }
  }
}
</script>
