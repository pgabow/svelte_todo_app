<script lang="ts">
  import { todos } from '../../store/TodoStore'
  import TodoInput from './TodoInput.svelte';

console.log('Section',todos)
</script>

<section class="mt-8 space-y-4">
  {#each $todos as todo (todo.id)}
    <TodoInput {todo}/>
  {/each}

</section>