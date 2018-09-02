<template>
  <div class="row">
    <app-new-quote></app-new-quote>
    <app-quote v-for="quote in quotes">{{ quote }}</app-quote>
  </div>
</template>

<script>
  import Quote from './Quote.vue';
  import NewQuote from './NewQuote.vue';
  export default{
    props: ['quotes'],
    components: {
      appQuote: Quote,
      appNewQuote : NewQuote
    }
  }
</script>

<style>
</style>
