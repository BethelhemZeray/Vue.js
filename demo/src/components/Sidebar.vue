<template>
  <aside class="sidebar">
    <h2>My Dashboard</h2>
    <ul>
      <li>🏠 Home</li>
      <li>📊 Reports</li>
      <li>⚙️ Settings</li>
    </ul>
  </aside>
</template>

<script>
export default { name: "Sidebar" }
</script>

<style>
.sidebar {
  width: 220px;
  background: #1e293b;
  color: white;
  padding: 20px;
}
.sidebar h2 {
  margin-bottom: 20px;
}
.sidebar ul {
  list-style: none;
  padding: 0;
}
.sidebar li {
  margin: 10px 0;
  cursor: pointer;
}
.sidebar li:hover {
  color: #38bdf8;
}
</style>
