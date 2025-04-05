<script setup>
import HeaderComponent from "@/components/HeaderComponent.vue";
import GalleryComponent from "@/components/GalleryComponent.vue";
import ContactsComponent from "@/components/ContactsComponent.vue";
</script>

<template>
  <section id="top"></section>
  <header>
    <HeaderComponent />
  </header>
  <main>
    <section>
      <h1>
        Graphic Designer Portfolio
      </h1>
      <h2>
        by Artur Smykal
      </h2>
    </section >
    <section id="gallery">
      <GalleryComponent />
    </section>
    <section id="Contacts">
      <ContactsComponent />
    </section>
  </main>
  <footer>
    <p>@2025 Artur Smykal</p>
  </footer>
</template>

<style scoped>
header {
  position: sticky;
  top: 0;
  z-index: 1000;
}
main {
  margin: 3rem auto;
  max-width: 1200px;
}

h2 {
  animation: colorShift 5s infinite alternate;
  color: var(--vt-c-white);
}

footer {
  height: 3rem;
  background-color: #222222;
  display: flex;
  justify-content: center;
  align-items: center;
}

@keyframes colorShift {
  0% {
    color: var(--vt-c-orange);
  }
  50% {
    color: var(--vt-c-white);
  }
  100% {
    color: var(--vt-c-orange);
  }
}

@media (max-width: 1250px) {
  main {
    width: 90%;
  }
  footer {
    height: 2rem;
  }
}

</style>
