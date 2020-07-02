<template>
  <header class="header">
    <h1>TodoList</h1>
    <div id="nav">
      <RouterLink to="/">
        Home
      </RouterLink><RouterLink to="/about">
        About
      </RouterLink>
    </div>
  </header>
</template>

<script>
export default {
    name:"Header"
}
</script>

<style scoped>
    .Header {
        background: #333;
        color: #fff;
        text-align:center;
        padding: 10px;
}

    .Header a {
        color: #fff;
        padding-right: 5px;
        text-decoration: none;
}

</style>
