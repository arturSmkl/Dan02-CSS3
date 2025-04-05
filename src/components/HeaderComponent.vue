<script setup>

</script>

<template>
  <div class="header-container">
    <a href="#top">
      <div class="logo"></div>
    </a>
    <nav>
      <a href="#gallery">
        Gallery
      </a>
      <a href="#Contacts">
        Contacts
      </a>
    </nav>
  </div>
</template>

<style scoped>
  .header-container {
    width: 100%;
    height: 4rem;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
    background-color: #222222;
    box-shadow: 0 1px 8px 0 rgba(255, 255, 255, 0.5);
  }

  .header-container .logo {
    background-image: url("src/assets/logo.png");
    background-size: cover;
    width: 3rem;
    height: 3rem;
    margin-left: 1rem;
  }

  .header-container nav {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
  }

  .header-container nav a {
    margin-right: 2rem;
    text-align: center;
    color: var(--vt-c-text-dark-1);
    font-weight: bold;
    text-decoration: none;
  }
  .header-container nav a:hover {
    color: var(--vt-c-white-soft);
  }
</style>