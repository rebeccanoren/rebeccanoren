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
		content="UX Case Study: How I used design process methods to deliver results to TRR."
	/>
</svelte:head>

<section>
	<img src={srcHero} class="hero rounded" alt="People standing infront of whiteboard" />
	<div class="container">
		<div class="description">
			<h1>Helping employers finding talent</h1>
			<p>
				TRR wanted to improve their current offerings to employers and explore opportunities in the
				digital context.
			</p>
			<p>
				In 2019, TRR offerings to employers mostly consisted of helping with handling redundancies
				and helping them find candidates to recruit. But TRR realized they could do more with their
				knowledge about the labor market and being experts in employment transitions. Therefore, my
				team was formed with the goal to identify these opportunities and execute on them. Our
				process was something like the following:
			</p>
			<h2 id="1">Start with basic understanding of the users</h2>
			<p>
				At the time, TRR lacked an understanding of the employer’s most important needs and there
				was no previous research to start from.
			</p>
			<p>
				I started with interviewing 20 representatives to create reliable and realistic
				representations of the target group. The interviews were analyzed and the findings were
				represented by five personas to describe the different needs, goals, attitudes and behavior
				patterns.
			</p>

			<figure>
				<img
					src={srcHero}
					class="box-shadow rounded"
					alt="The team having a workshop to get to know our personas."
				/>
				<figcaption>Workshop session to get to know our personas.</figcaption>
			</figure>

			<p>
				The opportunities we identified were endless, there were so many things we could do.
				Therefore, we needed to narrow our focus to a primary persona which was considered to be the
				most valuable for TRR. We ended up with HR managers at medium to large companies, it was a
				group TRR wanted to maintain good relationships with.
			</p>

			<h2 id="2">Identify the right opportunity</h2>
			<p>
				As a next step, I facilitated several workshops with stakholders to further explore the
				needs of our primary persona in detail. I facilitated impact mapping sessions to define our
				wanted effects. The idea was to visualize the reasoning from the effects we want to achieve
				to the user's needs. In this way, we were able to explore what we could do to support the
				defined goals.
			</p>

			<h2 id="3">Explore and try out ideas</h2>
			<p>
				At this point we decided to focus on the key persona’s need to recruit new, qualified and
				competent staff. To explore different ideas to meet this goal we decided to use the method
				Design Sprint. I facilitated the team and our stakeholders during the five day process where
				we explored and tested ideas. When we reached the end of the sprint, we had one tested
				prototype and a bunch of new hypotheses which we needed to evaluate further.
			</p>
			<figure>
				<img
					src={srcDesignSprint}
					class="box-shadow rounded"
					alt="Gif showing collaboration in Miro."
				/>
				<figcaption>Collaborating in a virtual Design Sprint session.</figcaption>
			</figure>
			<h2>The winning idea</h2>

			<p>
				The idea which got the most votes was to let employers search for jobseekers online based on
				the requirements of the position. We wanted to match employers with job-seekers allowing
				companies to search for competence among TRRs wide range of candidates.
			</p>

			<h2 id="5">Get feedback, refine</h2>
			<p>
				We improved the prototypes and included more refined ideas as we went. When evaluating, we
				found support for the idea was interesting to a couple of the employers. The idea was mostly
				popular with employers with a need to recruit competencies that are hard to find. The HR
				managers stated they saw great benefits getting in touch with candidates through TRR before
				they reached the official labor market. We also found the idea popular among recruitment
				agencies, they saw benefits with a unique access to a candidate pool.
			</p>
			<h2 id="5">Develop something small</h2>
			<p>
				Our goal was to develop a first iteration of the service with only the most important
				features. Therefore, our work with evaluating and refining the ideas with the target users
				continued after the Design Sprint. We wanted to examine which features were the most
				important and how the service would fit in the day to day work.
			</p>
			<p>
				We worked with hypotheses and evaluated them iteratively through user tests with prototypes
				and user interviews. Some of the findings are described below:
			</p>
			<ul class="margin">
				<li>
					Employers wanted to find candidates with industry specific competencies. Some of the
					examples of competencies were programming languages or knowledge in healthcare systems.
				</li>
				<li>
					One important need from recruiters was to quickly evaluate if the candidate is a good fit
					to the role and the company. Many recruiters wanted to review the career goals of the
					candidates before considering contacting them.
				</li>
				<li>
					The recruiters have must-have and nice-to-have traits when looking for candidates. They
					start with applying search filters for the dream candidate and then remove the
					nice-to-have traits when they don’t receive any search results. It’s essential for the UI
					to quickly respond with the matching candidates, not keeping the user waiting.
				</li>
			</ul>
			<p>The development of the service was conducted iteratively.</p>
			<h2 id="7">Present the right candidates</h2>
			<p>
				A big challenge was to make sure the results of the search were perceived as relevant to
				recruiters. We needed to figure out if we should present candidates which fulfilled:
			</p>
			<ul>
				<li>All of the criterias</li>
				<li>At least one criteria from each category</li>
				<li>Any of the criterias</li>
			</ul>
			<p>
				We also explored different solutions to this challenge. We tried to separate the search
				results list in two, one with candidates who fulfilled all of the criteria and a second
				where we included the candidates who were missing some criterias. I’m the second one, the
				missing criterias were also highlighted to allow the user to quickly evaluate whenever to
				consider the candidate.
			</p>

			<h2 id="6">Result</h2>
			<p>
				We had a first basic version of the service almost ready to be released to the end users
				when we ran into big trouble. The management team hit the pause button before release to
				employers. To not go into further details, there were other priorities in the organization
				affecting our project. The short term goal shifted and we should instead release the first
				version to allow employers to use the system as an internal tool. I felt disappointed. After
				all the work my team and I had put into optimizing the service for employers, we were
				looking forward to welcoming our first users. I still regard this project to be a failure of
				mine. Yet, I find a lot of positive outcomes from my work:
			</p>
			<ul class="margin">
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
					Showing the power of design where we showed the organization how to develop meaningful and
					valuable services using a user-centered approach.
				</li>
				<li>
					A great service to continue to develop together with the users. We found great support
					from our user research that employers couldn’t wait to start using our service.
				</li>

				<div class="infobox rounded">
					<h2 id="7">About TRR</h2>
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
				<h3>Keywords</h3>
				<ul>
					<li>Consumer facing</li>
					<li>Design Sprint</li>
					<li>User Testing</li>
				</ul>
			</div>

			<div class="navigation rounded box-shadow">
				<h5>Contents</h5>
				<ul>
					<li><a href="#1">User research</a></li>
					<li><a href="#2">Workshops with stakeholders</a></li>
					<li><a href="#3">Design Sprint</a></li>
					<li><a href="#5">Development</a></li>
					<li><a href="#6">Result</a></li>
					<li><a href="#7">About TRR</a></li>
				</ul>
			</div>
		</div>
	</div>
</section>

<style>
</style>
