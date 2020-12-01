<template>
  <div>
    this is the home page
  </div>
</template>

<script>
export default {
  fetch ({ params, redirect }) {
    redirect(301, '/about')
  }
}
</script>
