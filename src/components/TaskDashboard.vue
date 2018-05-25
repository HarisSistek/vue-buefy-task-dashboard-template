<template>
  <div>
    <section class="hero is-primary">
      <div class="hero-body">
        <div class="container">
          <h1 class="title">
            Task Dashboard
          </h1>
          <h2 class="subtitle">
            Shows utilization of agents and tasks
          </h2>
        </div>
      </div>
    </section>

    <br>

    <Overview></Overview>

    <Search></Search>

    <TaskTabs></TaskTabs>
  </div>
</template>

<script>
  import Overview from "./Overview";
  import TaskTabs from "./TaskTabs";
  import Search from "./Search";
  export default {
    name: 'TaskDashboard',
      components: {Overview, TaskTabs, Search},
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
