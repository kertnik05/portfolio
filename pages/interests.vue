<template>
  <section class="resume-section">
    <div class="resume-section-content">
      <h2 class="mb-5">
        {{ title }}
      </h2>
      <p>
        Apart from being a web developer, I enjoy most of my time being outdoors.
        During the warmer months, I enjoy mountain climbing, and cycling.
      </p>
      <p class="mb-0">
        When forced indoors, I follow a number of sci-fi and fantasy genre movies and
        television shows, I am an aspiring musician, and I spend a large amount of my free
        time exploring the latest technology advancements in the front-end web development
        world.
      </p>
    </div>
  </section>
</template>

<script>
export default {
  data () {
    return {
      title: 'Interests'
    }
  },

  head () {
    return {
      title: `${this.title} | Nikko Lumahang`
    }
  }
}
</script>
