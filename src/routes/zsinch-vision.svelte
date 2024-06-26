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
			<p class="xs">Sinch (2023)</p>
			<h1 class="xl">Defining the vision for Sinch Enterprise Platform</h1>
			<p class="s">
				In late 2022, I embarked on a project to envision the future state of the Sinch Enterprise
				platform. The primary objectives were to align patterns across the dashboard, enhance the
				user experience, and reduce complexity. The current user experience was disjointed due to
				teams working in isolation. This resulted in difficulties for users when performing complex
				tasks such as integrating with SMS APIs, managing API keys, and purchasing numbers.
			</p>

			<div class="summary rounded">
				<p>Summary</p>
				<p>
					As the UX Design Lead, I took charge of driving the exploration and vision-setting process
					for the future Sinch Enterprise platform. Working alongside multiple teams and
					stakeholders, I facilitated collaborative sessions and discussions to gather insights and
					align on design goals. Through close collaboration with developers, designers, and product
					managers, I synthesized inputs and integrated user feedback to inform the design
					direction.
				</p>
			</div>

			<h2 class="m" id="Part1">Part I: Understanding the current state</h2>
			<p>
				Through extensive user research, I delved into various aspects, including onboarding,
				product usage, and overall architecture. By carefully analyzing user feedback, I identified
				recurring issues, bottlenecks, and areas of confusion that required attention. Some of the
				insights included:
			</p>

			<h3>Difficult to get started</h3>
			<p>
				Users encountered difficulties when initially engaging with the platform and products such
				as SMS, Conversation API, and Voice API. The onboarding process was perceived as
				challenging, creating obstacles for users in effectively navigating and utilizing the
				products.
			</p>

			<h3>Lack of coherent user journey</h3>
			<p>
				Disjointed user journey within the platform, where different products and features lacked a
				cohesive flow. This resulted in confusion and significantly increased the learning curve for
				users in accomplishing their goals.
			</p>

			<h3>Inconsistent interface and design patterns</h3>
			<p>
				The platform suffered from inconsistencies in interface design and user interface patterns,
				causing users to struggle with familiarity and cognitive load. Users found it challenging to
				understand common patterns and had to repeatedly adapt to different interfaces when
				interacting with various features.
			</p>

			<figure>
				<img
					src={srcApiToken}
					class="box-shadow rounded"
					alt="Illustrating a developer struggeling to find the API token"
				/>
				<figcaption>
					Presentation slide from User Research Findings, developers struggles to find the API
					token.
				</figcaption>
			</figure>

			<div class="divider">
				<img src={srcDivider} alt="Divider svg" />
			</div>
			<h2 class="m" id="Part2">Part II: The Design Challenge</h2>

			<p>
				The objective of our efforts was to address the problems identified through research. Our
				primary goals were to simplify the onboarding process, provide clearer guidance, reduce
				friction, and create a cohesive user journey. By achieving these goals, we aimed to enhance
				the overall user experience and improve user satisfaction with the platform.
			</p>
			<p>
				Furthermore, the challenge centers around the implementation of the new account model as the
				fundamental pillar of the architecture. This new model is designed to support large
				organizations, prioritizing robust access control. To overcome this challenge, platform's
				structure need to be enhanced by necessary adjustments.
			</p>

			<p>To address these challenges, I identified the following How might we statements:</p>

			<ul class="margin">
				<li>
					How might we streamline the onboarding process to make it easier for users, including
					individual developers and large organizations, to get started and effectively navigate our
					platform and products?
				</li>

				<li>
					How might we create a cohesive user journey within the platform that seamlessly integrates
					different products and features, reducing confusion and minimizing the learning curve for
					users?
				</li>

				<li>
					How might we establish consistent interface design and user interface patterns across the
					platform to enhance familiarity, improve usability, and reduce cognitive load for users?
				</li>
			</ul>

			<h2 class="m" id="Part2">Part III: Benchmarking & Inspiration</h2>

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
				<img src={''} class="box-shadow rounded" alt="Wireframes showing search UI with filters" />
				<figcaption>Wireframe of the final product's basic functionality.</figcaption>
			</figure>

			<figure class="small">
				<img
					src={''}
					class="box-shadow rounded"
					alt="Wireframes showing presentation of a candidate"
				/>
				<figcaption>Presentation of a candidate's profile.</figcaption>
			</figure>

			<div class="infobox rounded" id="About-Sinch">
				<p>About TRR</p>
				<p>
					TRR is a non-profit foundation. They work with with employment transitions and working
					life, contributing to learning and mobility in the Swedish labor market. Their activities
					are aimed at companies in the private labor market, trade union representatives, and
					company employees. <a href="https://www.trr.se/">Learn more about TRR.</a>
				</p>
			</div>
		</div>

		<div class="sidebar">
			<div class="navigation rounded box-shadow blur">
				<p>Table of contents</p>
				<ul>
					<li><a href="#Part1">Part I: Understanding the current state</a></li>
					<li><a href="#Part2">Part II: The Design Challenge</a></li>
					<li><a href="#Part3">Part III: Benchmarking & Inspiration</a></li>
					<li><a href="#Result">Result</a></li>
					<li><a href="#About-Sinch">About Sinch</a></li>
				</ul>
			</div>
		</div>
	</div>
</section>

<style>
</style>
