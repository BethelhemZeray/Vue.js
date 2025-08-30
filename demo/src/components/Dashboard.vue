<template>
  <div class="dashboard-content">
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
  padding: 10px;
}
.cards {
  display: flex;
  gap: 20px;
}
.card {
  flex: 1;
  background: green;

}
</style>
