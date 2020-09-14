<template>
  <div>
    <h1 class="title">Todos</h1>
    <section class="todoapp">
      <div>
        <h1 class="loading">Loading...</h1>
      </div>
      <div>
        <header class="header">
          <input
            class="new-todo"
            autofocus
            autocomplete="off"
            v-model="newTodo"
          />
        </header>
      </div>
    </section>
  </div>
</template>
<script>
export default {
  name: "Todo",
  

  data () {
     return {
         newTodo: '',
     } 
  }
};
</script>
<style scoped>
.title {
  width: 100%;
  font-size: 80px;
  margin-bottom: 20px;
  line-height: 80px;
  font-weight: 100;
  text-align: center;
  color: black;
-webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-rendering: optimizeLegibility;
}
.loading {
  width: 100%;
  font-size: 40px;
  margin-bottom: 20px;
  line-height: 80px;
  font-weight: 100;
  text-align: center;
  color: black;
   -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-rendering: optimizeLegibility;
}
.new-todo {
    padding: 16px 16px 16px 60px;
    border: none;
    background: rgba(0, 0, 0, 0.003);
    box-shadow: inset 0 -2px 1px rgba(0,0,0,0.03);
}
</style>