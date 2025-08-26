<template>
  <div id="app" class="dashboard">
    <Sidebar />

    <div class="main-content">
      <Navbar />
      <div class="content-area">
        <Dashboard />
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import Sidebar from './components/Sidebar.vue'
import Navbar from './components/Navbar.vue'
import Dashboard from './components/Dashboard.vue'
</script>

<style>
/* Make app fill the whole viewport */
html, body, #app {
  height: 100%;
  width: 100%;
  margin: 0;
  padding: 0;
  font-family: sans-serif;
}

/* Dashboard container */
.dashboard {
  display: flex;
  height: 100vh; /* Full viewport height */
  width: 100vw;
  overflow: hidden;
}

/* Sidebar on left */
.sidebar {
  width: 240px;
  background: #1e293b;
  color: white;
  padding: 20px;
  display: flex;
  flex-direction: column;
}

/* Main content (Navbar + Dashboard) */
.main-content {
  flex: 1;
  display: flex;
  flex-direction: column;
  height: 100%; /* Fill remaining height */
  background: #f1f5f9;
}

/* Navbar fixed height */
.navbar {
  height: 60px;
  background: #f8fafc;
  padding: 15px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  border-bottom: 1px solid #e2e8f0;
}

/* Content area fills rest of main-content */
.content-area {
  flex: 1;               /* Fill remaining vertical space */
  padding: 20px;
  overflow-y: auto;      /* Scroll if content overflows */
  display: flex;
  flex-direction: column;
}
</style>
