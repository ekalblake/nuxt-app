<template>
  <div>
    <h1>Event #{{ id }}</h1>
  </div>
</template>

<script>
export default {
  head() {
    return {
      title: 'Event #' + this.id,
      meta: [
        {
          hid: 'descrpition',
          name: 'description',
          content: 'Qué quieres saber sobre el Evento #' + this.id,
        },
      ],
    }
  },
  computed: {
    id() {
      return this.$route.params.id
    },
  },
}
</script>

<style scoped></style>
