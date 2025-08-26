<template>
  <div class="dashboard-content">
    <h2>Overview</h2>
    <div class="cards">
      <div class="card">📈 Sales: $10,000</div>
      <div class="card">👥 Users: 250</div>
      <div class="card">✅ Tasks: 75%</div>
    </div>
  </div>
</template>

<script>
export default { name: "Dashboard" }
</script>

<style>
.dashboard-content {
  padding: 20px;
}
.cards {
  display: flex;
  gap: 20px;
}
.card {
  flex: 1;
  background: white;
  padding: 20px;
  border-radius: 10px;
  box-shadow: 0px 2px 6px rgba(0,0,0,0.1);
}
</style>
