<script setup xmlns="http://www.w3.org/1999/html">

</script>

<template>
  <div class="container">
    <h3>
      Contacts
    </h3>
    <div class="text-container">
      <div>
        Email<br>
        Phone Number<br>
        Instagram
      </div>
      <div style="text-align: right">
        example@email.xyz<br>
        123 456 789<br>
        @igusername
      </div>
    </div>
  </div>
</template>

<style scoped>

.container {
  width: 100%;
  background-color: var(--vt-c-orange);
  border-radius: 8px;
}

.text-container {
  width: 400px;
  display: flex;
  margin: 0 auto;
  padding-bottom: 2rem;
  flex-direction: row;
  justify-content: space-between;
}

</style>