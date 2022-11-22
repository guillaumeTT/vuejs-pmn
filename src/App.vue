<script setup>
import { RouterView } from 'vue-router'
</script>

<template>
      <h1>Calcul</h1>
    <div v-bind:id="app">
        <p>{{foo}}</p>
        <button class="btn" name="1">1</button>
        <button class="btn" name="2">2</button>
        <button class="btn" name="3">3</button>
        </div>
        <div>
        <button class="btn" name="4">4</button>
        <button class="btn" name="5">5</button>
        <button class="btn" name="6">6</button>
        </div>
        <div>
        <button class="btn" name="7">7</button>
        <button class="btn" name="8">8</button>
        <button class="btn" name="9">9</button>
        </div>
        <button class="btn" name="0">0</button>
        <button class="btn" name="+">+</button>
        <button class="btn" name="-">-</button>
        <button class="btn" name="/">/</button>
        <button class="btn" name="%">%</button>
        <button class="btn" name=".">.</button>
        <button class="btn" name="=">=</button>
        <button class="btn" name="C">C</button>

        <input type="text" />
  <RouterView />
</template>


<style scoped>
header {
  line-height: 1.5;
  max-height: 100vh;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 2rem;
}

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }

  nav {
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;

    padding: 1rem 0;
    margin-top: 1rem;
  }
}
</style>
