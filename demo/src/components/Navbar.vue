<template>
  <header class="navbar">
    <div class="nav-items">
      <button class="nav-btn source">
        <svg xmlns="http://www.w3.org/2000/svg" class="icon" fill="none" viewBox="0 0 24 24" stroke="currentColor">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 3v4h14V3H5zM5 11h14v10H5V11z" />
        </svg>
        Source
      </button>

      <button class="nav-btn filter">
        <svg xmlns="http://www.w3.org/2000/svg" class="icon" fill="none" viewBox="0 0 24 24" stroke="currentColor">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 4a1 1 0 011-1h16a1 1 0 011 1v2a1 1 0 01-.293.707L15 13.414V19a1 1 0 01-2 0v-5.586L3.293 6.707A1 1 0 013 6V4z" />
        </svg>
        Filter
      </button>

      <button class="nav-btn download">
        <svg xmlns="http://www.w3.org/2000/svg" class="icon" fill="none" viewBox="0 0 24 24" stroke="currentColor">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 4v16h16V4H4zm8 8l4-4m0 0l-4 4-4-4m4 4v8" />
        </svg>
        Download Report
      </button>
    </div>
  </header>
</template>

<script>
export default { name: "Navbar" }
</script>

<style scoped>
.navbar {
  display: flex;
  justify-content: flex-start;
  align-items: center;
  padding: 10px 20px;
  background-color: #ffffff;
  gap: 20px;
  box-sizing: border-box;
}


.nav-items {
  display: flex;
  gap: 15px;
}

.nav-btn {
  display: flex;
  align-items: center;
  gap: 6px;
  background-color: #f3f4f6;
  border: 1px solid #d1d5db;
  border-radius: 5px;
  padding: 6px 12px;
  cursor: pointer;
  font-size: 14px;
  transition: background 0.2s, color 0.2s;
}


.nav-btn.download {
  background-color: #22c55e; 
  color: white;
}

.nav-btn.download:hover {
  background-color: #16a34a; 
}


.nav-btn.filter {
  background-color: #d0d6d2ff; 
  color: black;
}
.nav-btn.source {
  color: black;
}



.icon {
  width: 18px;
  height: 18px;
  stroke: currentColor;
}
</style>
