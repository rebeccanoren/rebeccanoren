<script context="module">
	export const prerender = true;
</script>

<script>
	let srcHero = '/finding-talent/personas-ws.jpg';
	let srcDesignSprint = '/finding-talent/design.gif';
</script>

<svelte:head>
	<title>Helping employers finding talent</title>
	<meta
		name="description"
		content="UX Case Study: How I used design methods to deliver results to TRR."
	/>
</svelte:head>

<section class="case">
	<div class="intro">
		<p class="xs">TRR (2019)</p>
		<h1 class="xl">Helping employers hiring talent</h1>

		<p class="xs">Identifying opportunities through Design Thinking.</p>
	</div>
	<img src={srcHero} class="hero rounded" alt="People standing infront of whiteboard" />

	<div class="container">
		<div class="description">
			<p class="s">
				TRR wanted to improve their current digital offerings to employers. In 2019, TRR mostly
				helped with redundancy handling and recruiting candidates. However, TRR realized they could
				do more with their knowledge about the labor market and being experts in employment
				transitions. Therefore, my team was formed with the goal to identify these opportunities and
				execute on them.
			</p>

			<h2 class="m" id="Talk-to-employers">Part I: Talk to employers 🕵️‍♀️</h2>
			<p>
				I started with the basics: doing research. First months of the project, I interviewed 20
				representatives of the employers side. Then I analyzed those interviews to create five
				personas to describe users' needs, goals, attitudes and behavior patterns.
			</p>
			<p>
				It became clear that the possibilities were endless, and there was so much we could do to
				bring value to employers. Now we needed to find the one thing that would make the biggest
				impact on TRR's business. For us that meant narrowing our focus down to HR managers at
				medium-to-large companies.
			</p>
			<p>
				As a next step, I facilitated a series of workshops to delve deeply into the desires and
				needs of our primary persona. I facilitated impact mapping sessions to define our wanted
				effects and what we could do: how could we support their goals?
			</p>

			<figure>
				<img
					src={srcHero}
					class="box-shadow rounded"
					alt="The team having a workshop to get to know our personas."
				/>
				<figcaption>Workshop session to get to know our personas.</figcaption>
			</figure>

			<h2 class="m" id="Explore-ideas">Part II: Explore ideas 💡</h2>

			<p>
				At this point, we decided to address our primary persona's need for qualified employees. To
				explore different ideas to meet this goal, I facilitated a Design Sprint: a 5-day process
				where we explored and tested ideas. We had one tested prototype at the end of it, and a
				bunch of new hypotheses which we needed to evaluate further.
			</p>
			<figure>
				<img
					src={srcDesignSprint}
					class="box-shadow rounded"
					alt="Gif showing collaboration in Miro."
				/>
				<figcaption>Collaborating in a virtual Design Sprint session.</figcaption>
			</figure>
			<h2 class="m">The winner</h2>

			<p>
				The idea which got the most votes was to let employers search for jobseekers online based on
				the requirements of the position. We wanted to match employers with job-seekers allowing
				companies to search for competence among TRRs wide range of candidates.
			</p>

			<h2 class="m" id="Refinements">Part III: Refinements ♻️</h2>
			<p>
				We revised the prototypes and included more refined ideas as we went. We tested the idea
				with some employers, who found it interesting for recruiting competencies that are hard to
				find. HR managers saw great benefits in getting in touch with candidates through TRR before
				they reached the official labor market. Recruitment agencies also found value in a unique
				access to potential candidates.
			</p>

			<p>
				We wanted to develop a first iteration of the service with only the most important features.
				We continued to refine the functionality in parallel with development. We wanted to know
				what features were the most important and how the service would fit into the daily work.
			</p>
			<p>
				So we worked with hypotheses and evaluated them iteratively through user tests with
				prototypes and user interviews. From the research, we knew we needed to accomplish three
				things:
			</p>

			<ul class="margin">
				<li>
					Employers wanted to find candidates with industry specific competencies. For example,
					programming languages or industry specific software.
				</li>
				<li>
					We needed to make recruiters able to quickly evaluate if the candidate is a good fit to
					the role and the company. Many recruiters also told us they wanted to review the career
					goals of the candidates before considering contacting them.
				</li>
				<li>
					We needed to provide quick responses with the matching candidates, not keeping the user
					waiting when adding and removing search filters.
				</li>
			</ul>

			<h2 class="m">Present the right candidates</h2>
			<p>
				A big challenge was to make sure the results of the search were perceived as relevant to
				recruiters. We needed to figure out if we should present candidates who fulfills:
			</p>
			<ul>
				<li>All of the criterias</li>
				<li>At least one criteria from each category</li>
				<li>Any of the criterias</li>
			</ul>
			<p>
				We also explored different solutions to this challenge. We tried to separate the search
				results list in two, one with candidates who fulfilled all of the criteria and a second
				where we included the candidates who were missing some criterias. In the second one, the
				missing criterias were also highlighted to allow the user to quickly evaluate whenever to
				consider the candidate.
			</p>

			<h2 class="m" id="Result">Result</h2>
			<p>
				Although we had a first basic version of the service almost ready to be released, we hit
				some big trouble. Instead of releasing it to employers right away—which was our original
				plan— the management team postponed the launch of the service until employers could use it
				as an internal tool. This set us back, but I know that we did a lot of good work, and are
				proud of what we achieved:
			</p>
			<ul class="margin">
				<li>
					A recruitment tool to continue to develop together with the users. We found great support
					from our user research that employers couldn’t wait to start using our service.
				</li>
				<li>
					A base of extensive user research to build upon. The majority of the work I did was
					establishing a knowledge base for the organization to continue improving and identifying
					opportunities from.
				</li>
				<li>
					We were the first team at TRR to use the design sprint as a method to involve the
					stakeholders in the organization and solve problems together.
				</li>
				<li>
					Demonstrating the power of design where we showed the organization how to develop
					meaningful and valuable services using a user-centered approach.
				</li>

				<div class="infobox rounded">
					<h2 class="m" id="About-TRR">About TRR</h2>
					<p>
						TRR works with employment transitions and working life, contributing to learning and
						mobility in the Swedish labor market. Its activities are aimed at companies in the
						private labor market, trade union representatives and company employees. TRR is a
						non-profit foundation based on a collective agreement between the Confederation of
						Swedish Enterprise and PTK.
					</p>
				</div>
			</ul>
		</div>

		<div class="sidebar">
			<div class="keywords">
				<h3 class="2">Keywords</h3>
				<ul>
					<li>Consumer facing</li>
					<li>Design Sprint</li>
					<li>User Testing</li>
				</ul>
			</div>

			<div class="navigation rounded box-shadow">
				<h5 class="xs">Contents</h5>
				<ul>
					<li><a href="#Talk-to-employers">Part I: Talk to employers</a></li>
					<li><a href="#Explore-ideas">Part II: Explore ideas</a></li>
					<li><a href="#Refinements">Part III: Refinements</a></li>
					<li><a href="#Result">Result</a></li>
					<li><a href="#About-TRR">About TRR</a></li>
				</ul>
			</div>
		</div>
	</div>
</section>

<style>
</style>
