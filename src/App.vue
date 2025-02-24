<template>
  <h1>{{ message }}</h1>
  <hr />
  <h1>number: {{ number }}</h1>
  <hr/>
  <h1>double it = {{ doubleNumber(number) }}</h1>
  <hr/>
  <h1>{{ number > 150?'num bigger than 150':'less than 150' }}</h1>
  <hr/>
  <h1 v-text="number"></h1>
  <h1>{{ rawHtml }}</h1>
  <h1 v-html="rawHtml"></h1>
</template>

<script setup>
  let message = 'hello view'
  let number = 50

  function doubleNumber(num) {
    return num * 2
  }

  let rawHtml = '<span style="color: red">This should be red</span>'

</script>

<style lang="scss" scoped>

</style>