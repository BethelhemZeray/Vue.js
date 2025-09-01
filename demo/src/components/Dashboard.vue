<template>
  <div class="dashboard-content">
    <div class="cards">
      <div class="card">
        <div class="icon">📈</div>
        <div class="info">
          <div class="title">Total waiting list</div>
          <div class="value">43</div>
        </div>
      </div>

      <div class="card">
        <div class="icon">👥</div>
        <div class="info">
          <div class="title">New signups today</div>
          <div class="value">5</div>
        </div>
      </div>

      <div class="card">
        <div class="icon">✅</div>
        <div class="info">
          <div class="title">Top source</div>
          <div class="value">Linkeldn</div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default { name: "Dashboard" }
</script>

<style scoped>
.dashboard-content {
  padding: 10px;
}
.cards {
  display: flex;
  gap: 20px;
}
.card {
  flex: 1;
  color: white;
  margin: 10px;
  padding: 15px;
  border: 1px solid #d5dbe3ff;
  border-radius: 12px;
  display: flex;
  align-items: center; /* icon and info aligned in row */
  gap: 15px;
}

/* Icon styles */
.card .icon {
  font-size: 2.5rem;
  flex-shrink: 0; /* keep icon fixed size */
}

/* Info column */
.card .info {
  display: flex;
  flex-direction: column;
  justify-content: center;
  color: black;
  font: sans-serif;
}

/* Title styles */
.card .title {
  font-size: 1.2rem;
  font-weight: light;
  margin-bottom: 5px;
  color: black;
  
  font: sans-serif;
}

/* Value styles */
.card .value {
  font-size: 1.5rem;
  font-weight: bold;
  color: black;
}
</style>
