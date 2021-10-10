<template>
    <div id="app">
    <div class="main-wrapper">
      <part-navbar />
      <part-sidebar />
      <!-- Main Content -->
      <div class="main-content">
        <Nuxt />
      </div>
      <footer class="main-footer">
        <div class="footer-left">
          Copyright &copy; 2018 <div class="bullet"></div> Design By <a href="https://nauval.in/">Muhamad Nauval Azhar</a>
        </div>
        <div class="footer-right">
          2.3.0
        </div>
      </footer>
    </div>
  </div>
  
</template>
<script>
import sidebar from '../components/part/sidebar.vue';
import navbar from '../components/part/navbar.vue';
export default {
  components : {
    sidebar, navbar
  },
}
</script>