<template>
  <div class="max-w-[400px] m-auto">
    <Header />
    <Nuxt />
    <Footer />
  </div>
</template>

<script>
import Header from "./Header";
import Footer from "./Footer";
export default {
  components: {
    Header,
    Footer,
  },
};
</script>