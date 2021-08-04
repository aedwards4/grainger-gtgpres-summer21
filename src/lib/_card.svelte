<script>
	export let teamName;
	export let teamMembers;
</script>

<div class="card">
	<h3>{teamName}</h3>

	<div class="names">
		<ul>
			{#each teamMembers as name}
				<li>{name}</li>
			{/each}
		</ul>
	</div>
</div>

<style>
	.card {
		color: black;
		background-color: rgba(255, 255, 255, 0.2);
		padding-bottom: 10px;
		margin: 10px 10px;
		width: 250px;
		border-radius: 5px;
		vertical-align: middle;
		box-shadow: 0 15px 15px rgba(0, 0, 0, 0.5);
		height: 175px;
	}

	.card:hover h3 {
		background-color: rgba(152, 25, 26, 0.5);
		
	}

	h3 {
		padding: 5px 20px 5px 20px;
		text-transform: uppercase;
		text-align: center;
		background-color: rgba(255, 255, 255, 0.5);
		border-top-left-radius: 5px;
		border-top-right-radius: 5px;
		top: 0;
		margin-top: 0;
		vertical-align: middle;
		height: 50px;
		display: flex;
		justify-content: center;
		align-content: center;
		flex-direction: column;
	}

	ul {
		list-style: none;
		list-style-type: none;
		padding: 0;
		justify-content: center;
		text-align: center;
	}

	.names {
		display: flex;
		justify-content: center;
		align-content: center;
		flex-direction: column;
	}
</style>
