<script>
export default {
  data() {
    return {
      variable : {
        foo:"tert",
      res:"",
      btn:"1",
      }
        
      
    }
  },
  methods: {
    test : function(e){
      const btnVal = e.target.value;
      alert(""+e.target.value);
      return btnVal;
    },
    greet(event) {
    // `this` inside methods points to the current active instance
    alert(`Hello ${event.target.name}!`)
    // `event` is the native DOM event
    if (event) {
      foo += foo + event.target.name;
      return event.target.tagName
    }
  }
  }
}
</script>
<template>
      <h1>Calcul</h1>
    <div id="app">
        {{ variable.foo }}
        <button class="btn" v-on:click="greet" name="1">1</button>
        <input type="button" class="btn" v-model="all" data="text" />
        <button class="btn" @click="3" name="3">3</button>
        </div>
        <div>
        <button class="btn" @click="$test(4)" name="4">4</button>
        <button class="btn" @click="5" name="5">5</button>
        <button class="btn" @click="6" name="6">6</button>
        </div>
        <div>
        <button class="btn" @click="" name="7">7</button>
        <button class="btn" @click="" name="8">8</button>
        <button class="btn" @click="" name="9">9</button>
        </div>
        <button class="btn" @click="" name="0">0</button>
        <button class="btn" @click="" name="+">+</button>
        <button class="btn" @click="" name="-">-</button>
        <button class="btn" @click="" name="/">/</button>
        <button class="btn" @click="" name="%">%</button>
        <button class="btn" @click="" name=".">.</button>
        <button class="btn" @click="" name="=">=</button>
        <button class="btn" @click="" name="C">C</button>
        <p>Le message est : {{ variable.btn }}</p>
        <input type="text" :value="all" />
</template>


<style scoped>
header {
  line-height: 1.5;
  max-height: 100vh;
}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 2rem;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}


@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
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
