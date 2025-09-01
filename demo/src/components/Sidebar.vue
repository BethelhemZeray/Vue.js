<template>
  <aside :class="['sidebar', { collapsed }]">
    <ul class="menu">
      <li :class="{ active: active === 'general' }">
        <router-link to="/general" @click.native="active='general'">
          🏠 <span v-if="!collapsed">General</span>
        </router-link>
      </li>
      <li :class="{ active: active === 'statistics' }">
        <router-link to="/statistics" @click.native="active='statistics'">
          📊 <span v-if="!collapsed">Statistics</span>
        </router-link>
      </li>
      <li :class="{ active: active === 'waiting list' }">
        <router-link to="/waiting-list" @click.native="active='waiting list'">
          ⚙️ <span v-if="!collapsed">Waiting list</span>
        </router-link>
      </li>
      <li :class="{ active: active === 'admin' }">
        <router-link to="/admin" @click.native="active='admin'">
          ⚙️ <span v-if="!collapsed">Admin</span>
        </router-link>
      </li>
      <li :class="{ active: active === 'profile settings' }">
        <router-link to="/profile settings" @click.native="active='profile settings'">
          ⚙️ <span v-if="!collapsed">Profile settings</span>
        </router-link>
      </li>
    </ul>
  </aside>
</template>


<script setup lang="ts">
import { ref } from 'vue'

const collapsed = ref(false)
const active = ref('home')

function logout() {
  alert('Logging out...')
}
</script>

<style scoped>
/* Sidebar container */
.sidebar {
  width: 240px;
  color: white;
  display: flex;
  flex-direction: column;
  padding: 20px;
  transition: width 0.3s ease;
}

.sidebar.collapsed {
  width: 70px;
}

/* Header */
.sidebar-header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 30px;
  color: black;
}

.sidebar-header h2 {
  font-size: 1.2rem;
  margin: 0;
}

/* Menu lists */
.menu {
  list-style: none;
  padding: 0;
  margin: 0;
  flex-grow: 1;
}

.menu li {
  margin: 10px 0;
  display: flex;
  color: black;
  align-items: center;
  cursor: pointer;
  padding: 10px 12px;
  border-radius: 8px;
  transition: background 0.2s, color 0.2s;
}

.menu li span {
  margin-left: 10px;
}

/* Hover effect with box */
.menu li:hover {
  background: rgba(234, 239, 242, 0.93); 
}

/* Active item */
.menu li.active {
  background: rgba(227, 221, 233, 0.63);
  color: #717374ff;
  font-weight: bold;
}

/* Bottom section */
.menu.bottom {
  margin-bottom: auto;
  padding-top: 20px;
  border-top: 4px solid rgba(255,255,255,0.1);
}
</style>
