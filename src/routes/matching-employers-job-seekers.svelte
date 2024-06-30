<script context="module">
	export const prerender = true;
</script>

<script>
	let srcHero = '/finding-talent/personas-ws.jpg';
	let srcDesignSprint = '/finding-talent/design.gif';
	let srcCandidates = '/finding-talent/present-candidates.svg';
	let srcWireframes = '/finding-talent/wireframes.svg';
	let srcCandidate = '/finding-talent/candidate.svg';
	let srcDivider = 'divider.svg';

	let srcSinchOnboarding = '/sinch/onboarding/onboarding.svg';
	let enter1 = false;
</script>

<svelte:head>
	<title>Matching employers with job-seekers</title>
	<meta
		name="description"
		content="UX Case Study: How I used design methods to deliver results to TRR."
	/>
</svelte:head>

<section class="case">
	<div class="container">
		<div class="description">
			<p class="xs">TRR (2019)</p>
			<h1 class="xl">Matching employers with job-seekers</h1>
			<p class="s">
				In 2019, TRR mostly helped employers during redundancies and recruiting candidates. But TRR
				realized they could extend their offering to employers by improving their current digital
				offerings. Therefore, my team was formed with the goal to identify these opportunities and
				execute on them.
			</p>

			<div class="summary rounded">
				<p>Summary</p>
				<p>
					Working as the sole UX Designer in a team of developers and a product manager we created a
					search tool for recruiters to find qualified and competent staff. I had a leading role and
					facilitated the design process with the team. I did extensive user research, prototypes,
					UI and user tests.
				</p>
			</div>

			<h2 class="m" id="Talk-to-employers">Part I: Talk to employers 🕵️‍♀️</h2>
			<p>
				Initially, I conducted research by interviewing over 20 representatives from the employer
				side and developed 5 <a href="https://www.nngroup.com/articles/persona/">personas</a> based on
				their needs, goals, attitudes, and behavior patterns. From this research, it became clear that
				there was significant potential for improvement to increase the value delivered to employers
				and their employees.
			</p>
			<p>
				To prioritize our efforts, our product manager identified HR managers at medium-to-large
				companies as the primary target represented by one of the personas. I then facilitated
				workshops to further explore the needs and desires of this persona, using <a
					href="https://www.inuse.se/read/many-faces-impact-mapping/">Impact Mapping</a
				>
				sessions to identify key objectives and actions. Some of the challenges expressed in the persona
				was:
			</p>

			<ul>
				<li>Reskilling and upskilling employees</li>
				<li>Managing organizational changes</li>
				<li>Recruitment of the right candidates</li>
			</ul>

			<figure>
				<img
					src={srcHero}
					class="box-shadow rounded"
					alt="The team having a workshop to get to know our personas."
				/>
				<figcaption>Workshop session to get to know our personas.</figcaption>
			</figure>

			<div class="divider">
				<img src={srcDivider} alt="Divider svg" />
			</div>
			<h2 class="m" id="Explore-ideas">Part II: Explore ideas 💡</h2>

			<p>
				The Product Manager determined that our primary persona's need for hiring qualified
				employees required a solution. To address this challenge, I facilitated a remote
				<a href="http://www.gv.com/sprint/">Design Sprint</a>
				and invited the developers, the Product Manager, and other relevant stakeholders. Since the participants
				were located remotely, we used
				<a href="http://www.gv.com/sprint/">Miro</a> as a collaboration tool to ensure that everyone
				had an equal opportunity to contribute.
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
				After voting, the idea that received the most support was a recruitment tool for employers.
				Our goal was to match the competencies required by employers with qualified job-seekers from
				TRR's extensive pool of candidates.
			</p>

			<p>
				To test the prototype, I evaluated the main concept's viability by conducting tests with 5
				HR managers. Our riskiest assumption was that HR managers would be interested in recruiting
				job-seekers from TRR. The focus of the test was to determine if HR managers would use the
				recruitment tool in their daily work.
			</p>

			<p>
				Fortunately, the HR managers were enthusiastic about our proposed concept. They found it
				particularly useful for finding competencies that are difficult to find and saw a
				significant benefit in contacting candidates through TRR before they entered the official
				labor market.
			</p>

			<p>
				As a result of the Design Sprint, we developed a tested prototype and several new hypotheses
				that we needed to evaluate further.
			</p>

			<div class="divider">
				<img src={srcDivider} alt="Divider svg" />
			</div>

			<h2 class="m" id="Refinements">Part III: Refinements ♻️</h2>
			<p>
				Based on the feedback received, I revised the prototypes and included more refined ideas as
				we progressed. The prototype was further tested with employers, which revealed that
				recruitment agencies were also interested in gaining access to TRR's candidates.
			</p>

			<p>
				To develop the first iteration, we focused on including only the most essential features. At
				the same time, we continued to refine the functionality to determine which other features
				were most important and how the service could be seamlessly integrated into the user's daily
				work.
			</p>
			<p>
				To evaluate our hypotheses, we conducted iterative user tests with prototypes and user
				interviews. Based on our research, we identified three key goals that we needed to achieve:
			</p>

			<ul class="margin">
				<li>
					Enable employers to find candidates with industry-specific competencies, such as
					programming languages or industry-specific software.
				</li>
				<li>
					Allow recruiters to quickly evaluate whether a candidate is a good fit for both the role
					and the company. Many recruiters expressed a desire to review the career goals of
					candidates before considering reaching out to them.
				</li>
				<li>
					Provide search results at high speed to avoid making users wait when adding or removing
					search filters.
				</li>
			</ul>

			<h2 class="m">Present the right candidates</h2>
			<p>
				A big challenge was to make sure the results of the search were perceived as relevant to
				recruiters. We needed to figure out if we should present candidates who fulfills:
			</p>
			<ul>
				<li>All of the criterias.</li>
				<li>At least one criteria from each category.</li>
				<li>Any of the criterias.</li>
			</ul>
			<p>
				We explored different solutions to this challenge and talked to our target users. From my
				research we got the insight about recruiters often have a perfect profile with all the
				competencies required in the job description. In reality, it's difficult to find candidates
				who checks all the boxes.
			</p>

			<p>
				Therefore we decided to separate the search results list in two, one with candidates who
				fulfilled all of the criterias and a second where we included the candidates who were
				missing some criterias. In the second one, the missing criterias were also highlighted to
				allow the user to quickly evaluate the profiles.
			</p>

			<figure class="small">
				<img
					src={srcCandidates}
					class="box-shadow rounded"
					alt="Gif showing collaboration in Miro."
				/>
				<figcaption>Wireframe of the divided search results list.</figcaption>
			</figure>

			<div class="divider">
				<img src={srcDivider} alt="Divider svg" />
			</div>

			<h2 class="m" id="Result">Result</h2>
			<p>
				Although we had a first basic version of the service almost ready to be released, we hit
				some trouble. Instead of releasing it to employers right away, the management team postponed
				the launch. The reason was because the functionality for employers to sign in to TRR wasn't
				yet ready. A huge learning for me has been the importance of identifying all dependencies
				early on. Instead of releasing it right away to our target group, the management team
				decided to make it available as an internal tool. This was a set back for us, but I know
				that we did a lot of good work, and are proud of what we achieved:
			</p>
			<ul class="margin">
				<li>
					A simle and smooth UI for searching for candidates. The user research showed that
					employers couldn’t wait to start using our service.
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

			<figure class="small">
				<img
					src={srcWireframes}
					class="box-shadow rounded"
					alt="Wireframes showing search UI with filters"
				/>
				<figcaption>Wireframe of the final product's basic functionality.</figcaption>
			</figure>

			<figure class="small">
				<img
					src={srcCandidate}
					class="box-shadow rounded"
					alt="Wireframes showing presentation of a candidate"
				/>
				<figcaption>Presentation of a candidate's profile.</figcaption>
			</figure>

			<div class="infobox rounded" id="About-TRR">
				<p>About TRR</p>
				<p>
					TRR is a non-profit foundation. They work with with employment transitions and working
					life, contributing to learning and mobility in the Swedish labor market. Their activities
					are aimed at companies in the private labor market, trade union representatives, and
					company employees. <a href="https://www.trr.se/">Learn more about TRR.</a>
				</p>
			</div>

			<div class="next-case">
				<h3>Next up</h3>
				<a sveltekit:prefetch href="/sinch-getting-started">
					<figure
						on:mouseenter={() => {
							enter1 = !enter1;
						}}
						on:mouseleave={() => {
							enter1 = false;
						}}
						class="item"
					>
						<img
							src={srcSinchOnboarding}
							class="box-shadow border rounded-XL"
							alt="Design of Sinch Vision"
						/>
						<figcaption>
							<p class="uppercase xxs">Sinch (2024)</p>
							<h3 class="l nomargin {enter1 ? 'underline' : ''}">
								Getting started with Sinch SMS API
							</h3>
							<div class="tags">
								<span>User Research</span> <span>Usability</span> <span>Onboarding</span>
							</div>
						</figcaption>
					</figure>
				</a>
			</div>
		</div>

		<div class="sidebar">
			<div class="navigation rounded box-shadow blur">
				<p>Table of contents</p>
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
