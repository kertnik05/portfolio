<template>
  <section class="resume-section">
    <div class="resume-section-content">
      <h1 class="mb-0">
        Kert Rey Nikko
        <span class="text-primary">Lumahang</span>
      </h1>
      <div class="subheading mb-5">
        Purok 3, Pangyawan · Gitagum, Misamis Oriental 9020 · (+63) 965-402-0110 ·
        <a href="mailto:kertnik@gmail.com">kertnik@gmail.com</a>
      </div>
      <p class="lead mb-5">
        {{ description }}
      </p>
      <div class="social-icons">
        <a class="social-icon" href="https://www.linkedin.com/in/kertreynikko-lumahang">
          <i class="fab fa-linkedin-in" />
        </a>
        <a class="social-icon" href="https://github.com/kertnik05">
          <i class="fab fa-github" />
        </a>
        <a class="social-icon" href="https://twitter.com/kertnik">
          <i class="fab fa-twitter" />
        </a>
        <a class="social-icon" href="https://www.facebook.com/nikko.lumahang">
          <i class="fab fa-facebook-f" />
        </a>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data () {
    return {
      description: 'I am a highly resourceful, innovative, and competent PHP Laravel developer with extensive experience in the layout, design and coding of websites. Possessing considerable knowledge of the development of web and RESTful applications using PHP, VueJS and MySQL. I love working with technically strong team where I can solve complex problems with a good balance of freedom and responsibility.'
    }
  }
}
</script>

<style scoped>
a {
  text-decoration: none;
}
</style>
