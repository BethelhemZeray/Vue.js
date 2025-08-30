<template>
  <aside class="sidebar">
    <h2>My Dashboard</h2>
    <ul>
      <li>🏠 Home</li>
      <li>📊 Reports</li>
      <li>⚙️ Settings</li>
    </ul>
    <ul>
      <li>🔒 Logout</li>
      </ul>
  </aside>
</template>

<script>
export default { name: "Sidebar" }
</script>

<style>

.sidebar h2 {
  margin-bottom: 15px;
  color: black;
}
.sidebar ul {
  list-style: none;
  padding: 2;
}
.sidebar li {
  margin: 20px 0;
  color: black;
  cursor: pointer;
}
.sidebar li:hover {
  color: #38bdf8;
}
</style>
