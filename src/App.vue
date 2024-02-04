<script>
import Sidebar from "./Components/Sidebar.vue";
export default {
  components: {
    Sidebar,
  },
  data() {
    return {
      darkMode: true,
    };
  },
  methods: {
    toggleDarkMode() {
      this.darkMode = !this.darkMode;
      console.log("dark mode", this.darkMode);
    },
  },
};
</script>

<template>
  <div class="">
    <Sidebar :dark-mode="darkMode" @toggle-dark-mode="toggleDarkMode" />
  </div>
</template>

<style>
.app_heading_med {
  font-family: "Roboto", sans-serif;
  font-weight: 400;
  font-size: 15px;
  line-height: auto;
}
.app_heading_sm {
  font-family: "Roboto", sans-serif;
  font-weight: 400;
  font-size: 14px;
  line-height: auto;
  letter-spacing: 2px;
}
.app_body {
  font-family: "Roboto", sans-serif;
  font-weight: 300;
  font-size: 13px;
  line-height: auto;
}
.preview_h1 {
  font-family: "Roboto Slab", sans-serif;
  font-weight: 700;
  font-size: 32px;
  line-height: auto;
}
.preview_h2 {
  font-family: "Roboto Slab", sans-serif;
  font-weight: 300;
  font-size: 28px;
  line-height: auto;
}
.preview_h3 {
  font-family: "Roboto Slab", sans-serif;
  font-weight: 700;
  font-size: 24px;
  line-height: auto;
}
.preview_h4 {
  font-family: "Roboto Slab", sans-serif;
  font-weight: 700;
  font-size: 20px;
  line-height: auto;
}
.preview_h5 {
  font-family: "Roboto Slab", sans-serif;
  font-weight: 700;
  font-size: 16px;
  line-height: auto;
}
.preview_h6 {
  font-family: "Roboto Slab", sans-serif;
  font-weight: 700;
  font-size: 14px;
  line-height: auto;
}
.preview_p {
  font-family: "Roboto Slab", sans-serif;
  font-weight: 400;
  font-size: 14px;
  line-height: 24px;
}
.preview_p_bold {
  font-family: "Roboto Slab", sans-serif;
  font-weight: 700;
  font-size: 14px;
  line-height: 24px;
}
.preview_code {
  font-family: "Roboto Mono", sans-serif;
  font-weight: 400;
  font-size: 14px;
  line-height: 24px;
}
</style>
