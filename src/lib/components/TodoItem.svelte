<script>
    export let index;
    export let todo;
    export let editTodo;
    export let removeTodo;
</script>

<div class="todo">
    <p>
        {index + 1}. {todo}
    </p>
    <div class="actions">
        <i class="fa-regular fa-pen-to-square"></i>
        <i on:click={() => removeTodo(index)} class="fa-regular fa-trash-can"
        ></i>
    </div>
</div>

<style>
    .todo {
        border-left: 1px solid cyan;
        padding: 8px 14px;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
    .actions {
        display: flex;
        align-items: center;
        gap: 14px;
        font-size: 1.3rem;
    }
    .actions i {
        cursor: pointer;
    }
    .actions i:hover {
        color: coral;
    }
</style>
