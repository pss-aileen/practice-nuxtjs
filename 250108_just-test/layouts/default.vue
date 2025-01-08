<script setup lang="ts"></script>

<template>
  <div>
    <header>
      <h1>page title</h1>

      <nav>
        <ul>
          <li><NuxtLink to="/">HOME</NuxtLink></li>
          <li><NuxtLink to="/about">ABOUT</NuxtLink></li>
          <li><NuxtLink to="/contact">CONTACT</NuxtLink></li>
        </ul>
      </nav>
    </header>
    <slot></slot>
  </div>
</template>

<style scoped>
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background: #eee;
  padding: 16px;
  h1 {
    font-size: 16px;
  }

  nav {
    ul {
      list-style: none;
      padding: 0;
      display: block;
      font-size: 14px;
      margin: 0;

      li {
        display: inline-block;
      }

      li + li {
        margin-left: 16px;
      }
    }
  }
}
</style>
