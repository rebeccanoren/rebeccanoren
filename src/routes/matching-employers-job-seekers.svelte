<script context="module">
	export const prerender = true;
</script>

<script>
	let srcHero = '/finding-talent/personas-ws.jpg';
	let srcDesignSprint = '/finding-talent/design.gif';
</script>

<svelte:head>
	<title>Matching employers with job-seekers</title>
	<meta
		name="description"
		content="UX Case Study: How I used design methods to deliver results to TRR."
	/>
</svelte:head>

<section class="case">
	<div class="intro">
		<p class="xs">TRR (2019)</p>
		<h1 class="xl">Matching employers with job-seekers</h1>

		<p class="xs">
			How we developed a new service for a new target group by identifying opportunities and
			refining ideas.
		</p>
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
				I started with the basics: research. First months of the project, I interviewed 20
				representatives of the employers side. I analyzed those interviews to create five personas
				to describe users' needs, goals, attitudes and behavior patterns.
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
				At this point, the Product Manager decided to address our primary persona's need to find and
				hire qualified employees. To explore what we could to solve the problem, I facilitated a
				Remote <a href="http://www.gv.com/sprint/">Design Sprint.</a> I invited the developers in
				the team, the Product Manager and stakeholders in the organization who had insight about the
				challenge. We decided to use <a href="http://www.gv.com/sprint/">Miro</a> because we had participants
				from remote locations and wanted everyone to be able to contribute on equal terms.
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
				We voted and the idea that received the most votes was an idea about a recruitment tool for
				employers. The goal was to match employers' need for competencies with qualified candidates
				from the TRR's wide range of job-seekers. Leaving the design sprint, we had a tested
				prototype and a bunch of fresh hypotheses which we needed to evaluate further.
			</p>

			<h2 class="m" id="Refinements">Part III: Refinements ♻️</h2>
			<p>
				I revised the prototypes based on the feedback and included more refined ideas as we went. I
				continued to test the prototype with employers, who found it useful for recruiting
				competencies that are hard to find. HR managers saw a great benefit in getting in touch with
				candidates through TRR before they reached the official labor market. Recruitment agencies
				also found value in a unique access to potential candidates.
			</p>

			<p>
				We developed a first iteration of the service with only the most important features. We
				continued to refine the functionality in parallel with development. We wanted to know what
				features were the most important and how the service would fit in the user's daily work.
			</p>
			<p>
				The hypotheses was evaluated iteratively through user tests with prototypes and user
				interviews. From our research, we knew we needed to accomplish three things:
			</p>

			<ul class="margin">
				<li>
					Employers wanted candidates with industry specific competencies. For example, programming
					languages or industry specific software.
				</li>
				<li>
					Make it possible for recruiters to quickly evaluate if the candidate is a good fit for the
					role and the company. Many recruiters also told us they wanted to review the career goals
					of the candidates before considering contacting them.
				</li>
				<li>
					We needed to provide the search results at high speed, not keeping the user waiting when
					adding and removing search filters.
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
				We explored different solutions to this challenge and talked to our target users. From my
				research we got the insight about recruiters often have a perfect profile with all the
				competencies required in the job description. In reality, it's difficult to find a candidat
				who checks all the boxes.
			</p>

			<p>
				Therefore we decided to separate the search results list in two, one with candidates who
				fulfilled all of the criteria and a second where we included the candidates who were missing
				some criterias. In the second one, the missing criterias were also highlighted to allow the
				user to quickly evaluate the profiles.
			</p>

			<h2 class="m" id="Result">Result</h2>
			<p>
				Although we had a first basic version of the service almost ready to be released, we hit
				some big trouble. Instead of releasing it to employers right away — which was our original
				plan — the management team postponed the launch. The reason was because the functionality
				for employers to sign in to TRR wasn't yet ready. A huge learning for me has been the
				importance of identifying all dependencies early on. Instead of relasing it right away to
				our target group, the management team decided to make it available as an internal tool. This
				was a set back for us, but I know that we did a lot of good work, and are proud of what we
				achieved:
			</p>
			<ul class="margin">
				<li>
					A recruitment tool to continue to develop together with the users. We found great support
					from our user research that employers couldn’t wait to start using our service.
				</li>
				<li>
					A base of extensive user research to build upon. A huge part of the work I did was
					establishing a knowledge base for the organization to continue improving and identifying
					opportunities from.
				</li>
				<li>
					We were the first team at TRR to use the Design Sprint as a method to involve the
					stakeholders in the organization and solve problems together.
				</li>
				<li>
					Demonstrating the power of design where we showed the organization how to develop
					meaningful and valuable services using a user-centered approach.
				</li>
			</ul>

			<div class="infobox rounded">
				<h2 class="xs" id="About-TRR">About TRR</h2>
				<p>
					TRR is a non-profit foundation. They work with with employment transitions and working
					life, contributing to learning and mobility in the Swedish labor market. Their activities
					are aimed at companies in the private labor market, trade union representatives, and
					company employees. <a href="https://www.trr.se/">Learn more about TRR.</a>
				</p>
			</div>
		</div>

		<div class="sidebar">
			<div class="keywords">
				<h3 class="2">Keywords</h3>
				<ul>
					<li>Consumer facing</li>
					<li>User Interviews</li>
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
