<script>
	import Son from './son.svelte';
	import { liste } from './lesmusique.json';
	import App from './App.svelte';
	let classes =
		'w-full border-b-[1px] border-[rgb(255,255,255,0.3)] cursor-pointer';
</script>


<div class="h-[16rem] overflow-auto rounded-b-lg">
    {#each liste as musique}
    <Son {...musique}/>
{/each}
</div>

<style>
	::-webkit-scrollbar {
		width: 4px;
	}
	::-webkit-scrollbar-track {
		box-shadow: inset 0 0 5px grey;
		border-radius: 10px;
	}
	::-webkit-scrollbar-thumb {
		background: white;
		border-radius: 10px;
	}
</style>
