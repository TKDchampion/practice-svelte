<script>
	import VerticalList from './components/VerticalList.svelte';
	import HorizontalList from './components/HorizontalList.svelte';
	import Board from './components/Board.svelte';

	let items1 = [
		{ id: 11, name: 'item11' },
		{ id: 12, name: 'item12' },
		{ id: 13, name: 'item13' },
		{ id: 14, name: 'item14' },
		{ id: 15, name: 'item15' },
		{ id: 16, name: 'item16' },
		{ id: 17, name: 'item17' }
	];
	let items2 = [
		{ id: 21, name: 'item21' },
		{ id: 22, name: 'item22' },
		{ id: 23, name: 'item23' },
		{ id: 24, name: 'item24' },
		{ id: 25, name: 'item25' }
	];

	let board = [
		{
			id: 1,
			name: 'TODO',
			items: [
				{ id: 41, name: 'item41' },
				{ id: 42, name: 'item42' },
				{ id: 43, name: 'item43' },
				{ id: 44, name: 'item44' },
				{ id: 45, name: 'item45' },
				{ id: 46, name: 'item46' },
				{ id: 47, name: 'item47' },
				{ id: 48, name: 'item48' },
				{ id: 49, name: 'item49' }
			]
		},
		{
			id: 2,
			name: 'DOING',
			items: []
		},
		{
			id: 3,
			name: 'DONE',
			items: []
		}
	];
</script>

<VerticalList items={items1} />
<br />
<HorizontalList items={items2} containerWidth="50vw" />
<Board columnItems={board}></Board>

<style>
	:global(*) {
		box-sizing: border-box;
		margin: 0;
	}
</style>
