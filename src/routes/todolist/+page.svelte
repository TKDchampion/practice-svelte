<svelte:head>
	<title>Todo list</title>
	<meta name="description" content="Todo list" />
</svelte:head>

<script>
	import Todos from './components/Todos.svelte'
	import './styles.css';


	let todos = [
		{ id: 1, name: 'Create a Svelte starter app', completed: true },
		{ id: 2, name: 'Create your first component', completed: true },
		{ id: 3, name: 'Complete the rest of the tutorial', completed: false }
	]
</script>

<div class="text-column">
	<Todos {todos} />
</div>