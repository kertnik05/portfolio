<template>
  <nav id="sideNav" class="navbar navbar-expand-lg navbar-dark bg-primary fixed-top">
    <nuxt-link class="navbar-brand js-scroll-trigger" to="/">
      <span class="d-block d-lg-none">
        Kert Rey Nikko Lumahang
      </span>
      <span class="d-none d-lg-block">
        <img class="img-fluid img-profile rounded-circle mx-auto mb-2" src="~/assets/img/profile.jpg" alt="profile">
      </span>
    </nuxt-link>
    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent">
      <span class="navbar-toggler-icon" />
    </button>
    <div id="navbarSupportedContent" class="collapse navbar-collapse">
      <ul class="navbar-nav">
        <li class="nav-item">
          <nuxt-link class="nav-link" to="/about">
            About
          </nuxt-link>
        </li>
        <li class="nav-item">
          <nuxt-link class="nav-link" to="/experience">
            Experience
          </nuxt-link>
        </li>
        <li class="nav-item">
          <nuxt-link class="nav-link" to="/education">
            Education
          </nuxt-link>
        </li>
        <li class="nav-item">
          <nuxt-link class="nav-link" to="/skills">
            Skills
          </nuxt-link>
        </li>
        <li class="nav-item">
          <nuxt-link class="nav-link" to="/interests">
            Interests
          </nuxt-link>
        </li>
        <li class="nav-item">
          <nuxt-link class="nav-link" to="/projects">
            Projects
          </nuxt-link>
        </li>
      </ul>
    </div>
  </nav>
</template>

<script>
export default {

}
</script>
