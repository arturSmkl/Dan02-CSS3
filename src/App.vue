<script setup>
import HeaderComponent from "@/components/HeaderComponent.vue";
import GalleryComponent from "@/components/GalleryComponent.vue";
import ContactsComponent from "@/components/ContactsComponent.vue";
</script>

<template>
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
</template>

<style scoped>
header {
  max-width: 1920px;
  position: sticky;
  top: 0;
  z-index: 1000;
}
main {
  margin: 3rem auto;
  max-width: 1200px;
}

</style>
