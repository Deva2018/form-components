<template>
  <div>
  <label>Name </label>
  <label>{{username}}</label>
  <br>
  <label>Email </label>
  <label>{{email}}</label>
  <br>
  <label>Date of Birth </label>
  <label>{{dob}}</label>
  <br>
  <label>Mobile </label>
  <label>{{number}}</label>
  </div>
</template>

<script>

export default {
  name: 'component3',
  props: ['username','email','dob','number'],
};
</script>

<style scoped>

</style>
