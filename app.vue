<script setup lang="ts">
const title = `Carnival`
const description = ref('Carnival Description')
const name = `Carnival Name`

// This will be reactive when you change title/description above
useHead({
  title,
  meta: [{
    name: name,
    content: description
  }]
})
</script>

<template>
  <div class="hello">
    <Head>
      <Title>{{title}}</Title>
      <H2>Hello world</H2>
      <Meta name = name :content="description" />
    </Head>
  </div>
</template>

<style scoped>
.hello {
  font-family: Roboto, Helvetica, sans-serif;
  font-size: 3rem;
  padding: 2rem;
}
</style>
