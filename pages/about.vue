<template>
  <section class="resume-section">
    <div class="resume-section-content">
      <h1 class="mb-0">
        {{ first_name }}
        <span class="text-primary">
          {{ last_name }}
        </span>
      </h1>
      <div class="subheading mb-5">
        {{ street }} · {{ city }}, {{ province }} {{ zip_code }} · {{ contact_number }} ·
        <a :href="'mailto:'+email">
          {{ email }}
        </a>
      </div>
      <p class="lead mb-5">
        {{ description }}
      </p>
      <div class="social-icons">
        <a class="social-icon" :href="linkedin" target="_blank">
          <i class="fab fa-linkedin-in" />
        </a>
        <a class="social-icon" :href="github" target="_blank">
          <i class="fab fa-github" />
        </a>
        <a class="social-icon" :href="twitter" target="_blank">
          <i class="fab fa-twitter" />
        </a>
        <a class="social-icon" :href="facebook" target="_blank">
          <i class="fab fa-facebook-f" />
        </a>
        <a class="social-icon" :href="instagram" target="_blank">
          <i class="fab fa-instagram" />
        </a>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data () {
    return {
      first_name: 'Kert Rey Nikko',
      last_name: 'Lumahang',
      description: 'I am a highly resourceful, innovative, and competent PHP Laravel developer with extensive experience in the layout, design and coding of websites. Possessing considerable knowledge of the development of web and RESTful applications using PHP, VueJS and MySQL. I love working with technically strong team where I can solve complex problems with a good balance of freedom and responsibility.',
      street: 'Pangayawan',
      city: 'Gitagum',
      province: 'Misamis Oriental',
      zip_code: 9020,
      contact_number: '(+63) 965-402-0110',
      email: 'kertnik@gmail.com',
      linkedin: 'https://www.linkedin.com/in/kertreynikko-lumahang',
      github: 'https://github.com/kertnik05',
      twitter: 'https://twitter.com/kertnik',
      facebook: 'https://www.facebook.com/nikko.lumahang',
      instagram: 'https://www.instagram.com/kertniklum'
    }
  }
}
</script>

<style scoped>
a {
  text-decoration: none;
}
</style>
