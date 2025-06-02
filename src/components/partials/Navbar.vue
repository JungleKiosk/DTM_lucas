<script>
export default {
  name: "Navbar",
  components: {},
  data() {
    return {
      isDarkMode: false,
    };
  },
  mounted() {
    this.checkTheme();
    window.addEventListener("storage", this.syncTheme);
  },
  methods: {
    checkTheme() {
      const currentTheme = localStorage.getItem("theme");
      this.isDarkMode = currentTheme === "dark-mode";
    },
    syncTheme() {
      this.checkTheme();
    },
    toggleTheme() {
      this.isDarkMode = !this.isDarkMode;
      localStorage.setItem(
        "theme",
        this.isDarkMode ? "dark-mode" : "light-mode"
      );
      document.body.classList.toggle("dark-mode", this.isDarkMode);
      document.body.classList.toggle("light-mode", !this.isDarkMode);
    },
  },
};
</script>

<template>
  <nav class="navbar justify-content-center">
    <ul>
      <li>
        <router-link to="/">Home</router-link>
      </li>
      <li>
        <button @click="toggleTheme" class="btn btn-primary rounded-5">
          {{ isDarkMode ? "L" : "D" }}
        </button>
      </li>
    </ul>
  </nav>
</template>
