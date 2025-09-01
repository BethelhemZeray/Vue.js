<template>
  <div id="app" class="dashboard">
    <!-- Sidebar -->
    <Sidebar />

    <!-- Main content -->
    <div class="main-content">
      <!-- Navbar -->
      <Navbar />

      <!-- Dashboard (full width) -->
      <div class="content-section">
        <Dashboard />
      </div>

      <!-- First Content (full width) -->
      <div class="content-section">
        <Content />
      </div>

      <!-- Two side-by-side contents -->
      <div class="two-column">
        <div class="half-left">
          <ContentTwo />
        </div>
        <div class="half-right">
          <ContentThree />
        </div>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import Sidebar from './components/Sidebar.vue'
import Navbar from './components/Navbar.vue'
import Dashboard from './components/Dashboard.vue'
import Content from './components/Content.vue'
import ContentTwo from './components/ContentTwo.vue'
import ContentThree from './components/ContentThree.vue'
</script>

<style>
/* Reset and full viewport */
html,
body,
#app {
  height: 100vh;
  width: 100vw;
  margin: 0;
  padding: 0;
  font-family: sans-serif;
  background: #ffffff;
  overflow: hidden; 
  box-sizing: border-box;
}

/* Dashboard wrapper */
.dashboard {
  display: flex;
  height: 100vh;
  width: 100vw;
}

/* Sidebar */
.sidebar {
  width: 240px;
  flex-shrink: 0;
  border-right: 1px solid #e2e8f0;
  color: white;
  display: flex;
  flex-direction: column;
}

/* Main content */
.main-content {
  flex: 1;
  display: flex;
  flex-direction: column;
  height: 100%;
  overflow: hidden;
}

/* Navbar */
.navbar {
  height: 60px;
  padding: 0 15px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  background: #ffffff;
  flex-shrink: 0;
}

<style>
/* Each full-width content section */
.content-section {
  padding: 6px;          /* smaller inner padding */
  flex-shrink: 0;
  margin-bottom: 8px;    /* reduced vertical gap between sections */
}

/* Two-column layout */
.two-column {
  display: flex;
  gap: 10px;
  padding: 0 8px 8px 8px;
  flex: 1;
  height: 100%;
}

/* Left column */
.half-left {
  flex: 1;
  padding: 0;      /* no inner padding */
  height: 100%;
}

/* Right column */
.half-right {
  flex: 2;
  padding: 0;      /* no inner padding */
  height: 100%;
}

</style>