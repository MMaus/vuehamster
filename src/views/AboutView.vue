<template>
  <div class="about">
    <h1>This is an about page</h1>
    <span>Simple test cases</span>
    <div class="p-4 bg-purple-600 text-gray-100 rounded m-2">
      <Menu>
        <MenuButton>Menu </MenuButton>
        <MenuItems>
          <MenuItem v-slot="{ active }">
            <RouterLink
              to="/"
              :class="{ 'bg-blue-500': active }"
              class="font-bold"
              >Tracking</RouterLink
            >
          </MenuItem>
          <MenuItem v-slot="{ active }">
            <RouterLink to="/" :class="{ 'bg-blue-500': active }"
              >Overview</RouterLink
            >
          </MenuItem>
        </MenuItems>
      </Menu>
    </div>
  </div>
</template>
<script lang="ts" setup>
import { Menu, MenuItems, MenuItem, MenuButton } from "@headlessui/vue";
import { RouterLink } from "vue-router";
</script>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
    padding: 5em;
  }
}
</style>
