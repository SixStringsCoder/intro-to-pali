<script>
	import { createEventDispatcher } from 'svelte';

	const dispatch = createEventDispatcher();

  export let menuOptions = [];
	export let index;
</script>


<nav class="custom-select">
	<button id="prev-arrow" class="btn-arrow" on:click={() => dispatch('prev')}>&#8592;</button>

	<span class="custom-dropdown small">
    
    <select on:change bind:value={index}>
			<option value="" disabled>Go to section:</option> 
			{#each menuOptions as linkName, i}
		<option value={i}>{linkName}</option>
		{/each}
			</select>
		</span>

	
	<!-- <select on:change bind:value={index}>
		<option value="" disabled>Go to section:</option> 
			{#each menuOptions as linkName, i}
		<option value={i}>{linkName}</option>
		{/each}
	</select> -->
	
	<button id="next-arrow" class="btn-arrow" on:click={() => dispatch('next')}>&#8594;</button>
</nav>


<style>
	nav {
		margin: 10px 0 0 0 ;
		padding: 0;
		display: flex;
		justify-content: center;
		align-items: center;
	}

	/* custom select menu */
	.big {
		font-size: 1.2em;
	}

	.small {
		font-size: .7em;
	}

	/* Custom dropdown */
	.custom-dropdown {
		position: relative;
		display: inline-block;
		vertical-align: middle;
		margin: 10px; /* demo only */
	}

	.custom-dropdown select {
		background-color: #bc561b;
		color: #fff;
		font-size: inherit;
		padding: .5em;
		border: 0;
		margin: 0;
		border-radius: 3px;
		text-indent: 0.01px;
		text-overflow: '';
		-webkit-appearance: button; /* hide default arrow in chrome OSX */
	}

	.custom-dropdown::before,
	.custom-dropdown::after {
		content: "";
		position: absolute;
		pointer-events: none;
	}

	
	

	button.btn-arrow {
		background-color: hsl(41, 36%, 20%);
		color: white;
		margin: 0 10px;
		padding: 3px 5px 5px;
		font-size: 1.1rem;
		border-radius: 50%;
		cursor: pointer;
	}
	
	button.btn-arrow:active {
		background-color: hsl(22, 75%, 42%);
	}
</style>