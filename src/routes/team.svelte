<script>
	import Header from '/src/lib/_header.svelte';
	import Footer from '/src/lib/_footer.svelte';
</script>

<svelte:head>
	<title>My Team</title>
	<meta name="description" content="About the Core Engineering Experience team" />
</svelte:head>


<main>
	<Header />

	<section>
		<h2>Core Engineering Experience</h2>

		<h3>Our Vision</h3>
		<p style="margin-left: 20px;">We are an enablement team who provides self-service tooling and reusable patterns to other product engineer teams in order to support a consistent, seamless experience for our customers.</p>

		<h3>How We Do It</h3>
		<ol>
			<li class="order-li">An Opinionated Experience System Framework</li>
			<li class="order-li">The Grainger Design System</li>
			<li class="order-li">Experience System Composition Strategy and Architecture</li>
		</ol>

		<h3>My Manager and Mentor</h3>
		<ul>
			<li>Patrick Szczypinski – Engineering Manager</li>
		</ul>

		<h3>Our Team</h3>
		<ul>
			<li>Dave Braverman – TPM</li>
			<li>Claire Zhang – EBA</li>
			<li>Andy Freidenfelds – Tech Lead/Software Engineer, Front End</li>
			<li>Zev Goldberg – Software Engineer, Front End</li>
			<li>Bart Takuski – QA</li>
			<li>Ed Genne – QA</li>
			<li>Matt Leigh – UX Visual Designer</li>
			<li>Daran Redenbaugh – UX Visual Designer</li>
			<li>Chris Sienkiewicz – Engineering Director, Core and Native Apps</li>
		</ul>
	</section>

	<Footer />
</main>

<style>
	@import '$lib/global.css';

	h2 {
		/* font-family: 'Roboto', sans-serif; */
		font-family: 'Open Sans', sans-serif;
		font-size: 35px;
		text-align: center;
		margin-top: 5px;
	}

	h3 {
		font-size: 25px;
	}

	section {
		background-color: rgba(113, 113, 113, 0.7);
		box-shadow: 0 15px 15px rgba(0, 0, 0, 0.8);
		color: white;
		width: 75%;
		margin: 20px auto;
		padding: 20px;
		border-radius: 10px;
	}

	.order-li {
		padding: 5px 0;
	}
</style>
