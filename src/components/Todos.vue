<template>
  <div>
    <div
      v-for="(todo, index) in todos"
      :key="index"
    >
      <h3>{{ todo.title }}</h3>
            
      <TodoItem
        :todo="todo"
        @del-todo="$emit('del-todo',
                         todo.id)"
      />
    </div>
  </div>
</template>

<script>


export default {
    name: "Todos",
    components:{
      
},
    // eslint-disable-next-line vue/require-prop-types
    props: ["todos"]

}
</script>

<style scoped>

</style>