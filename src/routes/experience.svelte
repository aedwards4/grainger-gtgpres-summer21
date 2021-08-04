<script>
	import Header from '/src/lib/_header.svelte';
	import Footer from '/src/lib/_footer.svelte';
	import Card from '/src/lib/_card.svelte';

	const networking = [
		{
			teamName: 'Mobile',
			teamMembers: ['Jamie Thomason', 'Patrick McGoldrick']
		},
		{
			teamName: 'UI/UX',
			teamMembers: ['Daran Redenbaugh', 'Matt Leigh']
		},
		{
			teamName: 'ThoughtWorks',
			teamMembers: ['Scott Davis']
		},
		{
			teamName: 'Order History Experience',
			teamMembers: ['Clinton Bloodworth']
		},
		{
			teamName: 'Login & Registration',
			teamMembers: ['Scott Davies']
		},
		{
			teamName: 'KeepStock Experience',
			teamMembers: ['Joel Jackson', 'Tanvir Shaikh', 'Charles Currier', 'Mayra Vazquez']
		},
		{
			teamName: 'Cybersecurity',
			teamMembers: ['Deborah Barnes']
		},
		{
			teamName: 'Order History Capabilities',
			teamMembers: ['Rajesh Mulampaka', 'Fu-Chih Tu']
		},
		{
			teamName: 'Core Engineering Capabilities',
			teamMembers: ['Chris Lam', 'Noah Simon']
		},
		{
			teamName: 'Customer Data',
			teamMembers: ['Steve Chang', 'Bharath Guntur']
		},
		{
			teamName: 'Tech Talent Program',
			teamMembers: ['Paige Grons', 'Brian Kopiernicki', 'Jill Szpicki']
		}
	];
</script>

<svelte:head>
	<title>My Work Experience</title>
	<meta
		name="description"
		content="Description of my work that I've done while interning at Grainger"
	/>
</svelte:head>

<Header />

<input id="radio1" type="radio" name="css-tabs" checked />
<input id="radio2" type="radio" name="css-tabs" />

<div id="tabs">
	<label id="tab1" for="radio1">Technical</label>
	<label id="tab2" for="radio2">Networking</label>
</div>
<div id="content">
	<section id="content1">
		<h2>Technical</h2>

		<div class="tech-content">
			<div class="tech-section">
				<div class="heading">
					<h3>Design System Publication</h3>
					<p class="tech"><strong>Technologies:</strong> Svelte, HTML, CSS, Javascript</p>
				</div>
	
				<p>
					<h4>What I did:</h4>
					<ul>
						<li>Deployed 2 component pages, 
							<a href="http://design-system-dev.nonprod.graingercloud.com/components/checkbox" alt="Grainger Design System" target="_blank" rel="noopener">Checkbox and Text Inputs</a>, by replicating the design provided by UI/UX</li>
						<li>Created a custom Svelte component which may be used for future pages</li>
					</ul>
				<p>
					<h4>Why It's Important:</h4>
					<ul>
						<li>Promotes consistency</li>
						<li>Contributes to seamless user experience</li>
					</ul>
				
			</div>

			<div class="tech-section">
				<div class="heading">
					<h3>Experience System</h3>
					<p class="tech"><strong>Technologies:</strong> Svelte, HTML, CSS, Javascript</p>
				</div>

				<p>
					<h4>What I did:</h4>
					<ul>
						<li>Fixed positioning of check in Checkbox component</li>
						<li>Updated border style of Text Input component to match design standards</li>
					</ul>
				<p>
					<h4>Why It's Important:</h4>
					<ul>
						<li>Used by several teams</li>
						<li>Consistency promotes use</li>
					</ul>
			</div>

			<div class="tech-section">
				<div class="heading">
					<h3>Google Lighthouse & Accessibility</h3>
					<p class="tech"><strong>Technologies:</strong> Lighthouse, npm</p>
				</div>
				
				<p>
					<h4>What I did:</h4>
					<ul>
						<li>Added Google's Lighthouse dependency to Experience System</li>
						<li>Researched how to customize testing through the use of performance budgets</li>
					</ul>
				<p>
					<h4>Why It's Important:</h4>
					<ul>
						<li>Tracks metrics such as Performance, Accessibility, SEO, etc</li>
						<li>Inclusive design</li>
					</ul>
			</div>
		</div>

	
	</section>
	<section id="content2">
		<h2>Networking</h2>
		<div class="grid">
			{#each networking as instance}
				<Card {...instance} />
			{/each}
		</div>
	</section>
</div>


<Footer />

<style>
	@import '$lib/global.css';

	h2 {
		/* font-family: 'Roboto', sans-serif; */
		font-family: 'Open Sans', sans-serif;
		font-size: 35px;
		text-align: center;
		margin-top: 20px;
	}

	h3 {
		font-family: 'Open Sans', sans-serif;
		font-size: 25px;
		margin: 0;
	}

	h4 {
		font: 18px 'Open Sans', sans-serif;
		margin-bottom: 0;
		margin-top: 0;
		padding-left: 10px;
	}

	.heading {
		margin:0;
		background-color: rgba(255, 255, 255, 0.5);
		border-top-right-radius: 10px;
		border-top-left-radius: 10px;
		padding: 10px;
	}

	a {
		text-decoration: underline;
		color: black;
	}

	li {
		padding: 0 0 5px 0;
	}

	.grid {
		display: flex;
		flex-wrap: wrap;
		justify-content: center;
	}

	input[name='css-tabs'] {
		display: none;
	}

	#tabs {
		width: fit-content;
		margin-top: 20px;
		margin-bottom: 1px;
		margin-right: auto;
		margin-left: auto;
		background-color: rgba(113, 113, 113, 0.7);
		height: 40px;
		border-radius: 5px;
	}

	#tabs::after {
		content: '';
		display: block;
		position: absolute;
		z-index: 0;
		height: 40px;
		width: 127px;
		background: grey;
		transition: transform 400ms;
	}

	#tabs label {
		color: white;
		position: relative;
		z-index: 100;
		display: block;
		float: left;
		font-size: 18px;
		text-align: center;
		width: 125px;
		height: 100%;
		cursor: pointer;
		padding: 8px 0;
	}

	#radio1:checked ~ #tabs #tab1::before,
	#radio2:checked ~ #tabs #tab2::before {
		filter: invert(100%);
	}

	#radio1:checked ~ #tabs::after {
		transform: translateX(0);
		border-radius: 5px;
	}

	#radio2:checked ~ #tabs::after {
		transform: translateX(126px);
		border-radius: 5px;
	}

	#content {
		position: relative;
		height: 1200px;
		width: 75%;
		background-color: rgba(113, 113, 113, 0.7);
		color: white;
		margin: 0 auto 20px auto;
		padding: 0 20px;
		border-radius: 10px;
		box-shadow: 0 15px 15px rgba(0, 0, 0, 0.8);
	}

	#content::before {
		content: '';
		display: block;
		position: absolute;
		width: 0;
		height: 0;
		margin-left: -50px;
	}

	#content::after {
		content: '';
		display: block;
		position: absolute;
		width: 0;
		height: 0;
		margin-left: calc(100% + 30px);
	}

	#content section {
		position: absolute;
		transform: translateY(500px);
		opacity: 0;
		transition: transform 500ms, opacity 500ms;
	}

	#radio1:checked ~ #content #content1,
	#radio2:checked ~ #content #content2 {
		transform: translateY(0);
		opacity: 1;
	}

	.tech-content {
		width: 75%;
		margin: auto;
	}

	.tech-section {
		color: black;
		background-color: rgba(255, 255, 255, 0.2);
		border-radius: 10px;
		/* padding: 0 8px 2px 8px; */
		padding: 0 0 8px 0;
		margin: 20px 0;
		height: auto;
		box-shadow: 0 15px 15px rgba(0, 0, 0, 0.5);
	}

	#content1 {
		width: 97%;
	}

	.tech {
		margin-top: 5px;
		font-style: italic;
		margin-bottom: 0;
	}
	
</style>

