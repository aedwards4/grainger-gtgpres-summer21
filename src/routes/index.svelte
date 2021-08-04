<script>
	import Header from '/src/lib/_header.svelte';
	import Footer from '/src/lib/_footer.svelte';
</script>

<svelte:head>
	<title>About Me</title>
	<meta name="description" content="A quick introduction" />
</svelte:head>

<main>
	<Header />

	<section>
		<h2 class="intro">Hi, I'm Alexis!</h2>
		<div class="column-layout">
			<div class="column-1">
				<img src="IntroPic-1x.jpg" alt="Self Introduction" height="484px" width="265px" />
			</div>
			<div class="column-2">
				<ul>
					<li>Illinois Tech, May 2022</li>
					<li>Bachelor's and Master's in Computer Science</li>
					<li>New Orleans --> Chicago</li>
					<li>Cooking, Traveling, Biking, Reading</li>
				</ul>
			</div>
		</div>
	</section>

	<Footer />
</main>

<style>
	@import '$lib/global.css';

	main {
		background-image: url('background-img.png');
	}

	h2.intro {
		/* font-family: 'Roboto', sans-serif; */
		font-family: 'Open Sans', sans-serif;
		font-size: 35px;
		text-align: center;
		margin-top: 5px;
	}

	section {
		background-color: rgba(113, 113, 113, 0.7);
		box-shadow: 0 15px 15px rgba(0, 0, 0, 0.8);
		color: white;
		width: 75%;
		margin: 20px auto;
		padding: 20px;
		border-radius: 10px;
		text-align: center;
	}

	.column-layout {
		display: flex;
	}

	.column-1 {
		width: auto;
		padding-left: 20px;
		padding-right: 80px;
		margin: 0 50px;
	}

	.column-2 {
		flex: 50%;
		padding: 100px 0;
		margin-left: 0;
	}

	img {
		width: 100%;
		height: auto;
		border-radius: 5px;
	}

	li {
		font-family: 'Roboto', sans-serif;
		font-size: 30px;
		text-align: left;
		margin: 20px 0;
	}
</style>


<!-- Consistency important
	- When customer goes from eaxperience to exp on our site 
	- telling a story
	- imortant to have consistency
		- develops trust
		- lets them know they are on the same site 
	- only way teams know we have these is by visiting design sys public 
		- need to know how to use them
	- components only useful if people use them
		- can only happen if these pages exist 
	- more and more teams using these components
		- need a place to be able to get them
		- i built that place


Improved consistency in design 
	- Important that they're good and look right 
	- Illustrate the impact
		- component being used by 2 teams now and later 6-7
		- one change in that component sent it out to all teams using it
	- looks good and functions well
	- difficult to get people to use stuff we're building
		- not a captive aduience (cant make people use them)
		- best way is to educate them, publish design system, make sure they look good and work
	- changes made it look professional and so that ppl want to use them
		- if it looks broken, people wont use it

performance and accessibility are wildly important


allow other prod engineer teams to focus on needs of customer within their product domain -->