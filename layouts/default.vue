<template>
  <v-app :dark="darkMode" v-bind:class="theme === 'dark' ? 'dark-theme' : 'light-theme'">
    <!-- Navigation Drawer -->
    <v-navigation-drawer app v-model="drawer" :mini-variant="miniVariant">
      <v-list>
        <v-list-item to="" @mouseover="activeItem = 0" @mouseout="activeItem = null">
          <v-list-item-icon>
            <img
              :src="require('/assets/images/logo.png')"
              alt="Logo"
              class="v-icon mdi mdi-apps"
              style="max-width: 30px; max-height: 30px;"
            />
          </v-list-item-icon>
          <v-list-item-title v-show="activeItem === 0 && !miniVariant">Welcome</v-list-item-title>
        </v-list-item>

        <v-list-item to="/inspire" @mouseover="activeItem = 1" @mouseout="activeItem = null">
          <v-list-item-icon>
            <v-icon>mdi-chart-bubble</v-icon>
          </v-list-item-icon>
          <v-list-item-title v-show="activeItem === 1 && !miniVariant">Inspire</v-list-item-title>
        </v-list-item>

        <v-list-item to="/dashboard" @mouseover="activeItem = 2" @mouseout="activeItem = null">
          <v-list-item-icon>
            <v-icon>mdi-view-dashboard</v-icon>
          </v-list-item-icon>
          <v-list-item-title v-show="activeItem === 2 && !miniVariant">Dashboard</v-list-item-title>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>

    <!-- App Bar with fixed header -->
    <v-app-bar app v-bind:class="{ 'fixed-app-bar': scrollPosition > 0 }">
      <v-app-bar-nav-icon @click.stop="drawer = !drawer" />
      <v-toolbar-title>{{ title }}</v-toolbar-title>
      <v-spacer></v-spacer>
      <div>
        <v-icon @click="openMessageDialog" >mdi-message-text-outline</v-icon> <!-- Message icon -->
        <v-icon @click="openPersonDialog">mdi-account</v-icon> <!-- Person icon -->
      </div>
      <v-avatar @click="toggleTheme">
        <v-icon>mdi-weather-moon</v-icon>
      </v-avatar>
    </v-app-bar>

    <v-main>
      <v-container class="mt-5">
        <router-view></router-view>
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
export default {
  data() {
    return {
      darkMode: false,
      title: 'Your App Title',
      drawer: false,
      miniVariant: true,
      activeItem: null,
      theme: 'light', // Start with the light theme
      scrollPosition: 0, // Track the scroll position
    };
  },
  mounted() {
    window.addEventListener('scroll', this.handleScroll);
  },
  methods: {
    toggleTheme() {
      this.theme = this.theme === 'light' ? 'dark' : 'light';
    },
    handleScroll() {
      this.scrollPosition = window.scrollY;
    },
    openPersonDialog() {
      // Logic to open a person dialog
      // You can use a dialog component or other UI components for this.
    },
    openMessageDialog() {
      // Logic to open a message dialog
      // You can use a dialog component or other UI components for this.
    },
  },
};
</script>

<style scoped>
/* Dark theme styles */
.dark-theme {
  background-color: #333;
  color: #fff;
}

/* Light theme styles */
.light-theme {
  background-color: #fff;
  color: #333;
}

/* Sidebar with linear gradient background */
.v-navigation-drawer {
  background: black;
  color: #fff;
  /* Text color for the sidebar */
}

/* Header with a different linear gradient background */
.v-app-bar {
  background: black;
  color: #fff;
  /* Text color for the header */
}

/* Add this style for the fixed header */
.fixed-app-bar {
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  z-index: 100;
}



/* ... other styles */
</style>
