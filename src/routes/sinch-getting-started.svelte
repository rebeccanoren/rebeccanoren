<script context="module">
	export const prerender = true;
</script>

<script>
	let srcHero = '/sinch/vision/api-token.png';
	let srcUserJoruney = '/sinch/onboarding/user-journey.svg';
	let srcTime = '/sinch/onboarding/time.svg';
	let srcVideo = '/sinch/onboarding/API-key.mov';

	let srcCurrentdesign = '/sinch/onboarding/current-design.svg';
	let srcError = '/sinch/onboarding/error.png';
	let srcMotivation = '/sinch/onboarding/motivation.svg';
	let srcParameters = '/sinch/onboarding/parameters.svg';
	let srcInput = '/sinch/onboarding/input.svg';
	let srcAPIresponse = '/sinch/onboarding/API-response.svg';
	let srcSelectlanguage = '/sinch/onboarding/select-language.gif';
	let srcNewPage = '/sinch/onboarding/new-page.svg';
	let srcOptimalJourney = '/sinch/onboarding/optimal-journey.svg';
	let srcCompetitorresearch = '/sinch/onboarding/competitor-research.svg';
	let srcCompetitors = '/sinch/onboarding/competitors.svg';

	let srcApiToken = '/sinch/vision/api-token.png';
	let srcCandidates = '/finding-talent/present-candidates.svg';
	let srcWireframes = '/finding-talent/wireframes.svg';
	let srcCandidate = '/finding-talent/candidate.svg';
	let srcDivider = 'divider.svg';
</script>

<svelte:head>
	<title>Developers Getting started with Sinch SMS AP</title>
	<meta name="description" content="Developers Getting started with Sinch SMS API" />
</svelte:head>

<section class="case">
	<div class="container">
		<div class="description">
			<p class="xs">Sinch (2024)</p>
			<h1 class="xl">Developers Getting started with Sinch SMS API</h1>
			<p class="s">
				As Sinch adopts a Product-Led Growth (PLG) strategy, the focus has shifted towards
				optimizing the user experience, particularly for developers integrating our SMS API.
				Recognizing the critical role of a seamless onboarding process in driving user satisfaction
				and conversion rates, a new Onboarding Team was established. This team's primary objective
				is to streamline the journey for new sign-ups, enabling them to efficiently start using the
				SMS API and ultimately convert into paying customers.
			</p>

			<div class="summary rounded">
				<p>Summary</p>
				<p>
					As the UX Design Lead, I led my team to enhance the onboarding experience for Sinch's SMS
					API through user tests to identify pain points. With an agile approach, we improved the
					journey by making it easier to locate API parameters, enhancing documentation, and adding
					better error handling. These changes streamlined the onboarding process, reducing the time
					to "Aha-moment". The result was a smoother, more reliable experience, increasing user
					satisfaction and conversion rates. This is still an ongoing project.
				</p>
			</div>

			<h2 class="m" id="Part1">Part I: What is the current onboarding experience like?</h2>
			<h3>Sending a test SMS</h3>
			<p>
				I began by examining the current experience. I conducted 10 user tests with developers.
				These developers were tasked with using our SMS API to build a small application and send a
				test SMS to themselves using their code editor. By doing this, we could examine the entire
				journey and identify potential problems firsthand. This method allowed us to:
			</p>

			<ul class="margin">
				<li>
					Observing developers in a natural setting using their own code editors provided insights
					into how our API is utilized in real-world scenarios.
				</li>
				<li>
					Directly witnessing the challenges and frustrations developers faced helped us pinpoint
					specific areas that needed improvement.
				</li>
				<li>
					Developers provided immediate, candid feedback about their experience, enabling us to
					understand their perspectives and needs better.
				</li>
				<li>
					Assess how effectively our documentation and support resources assisted developers in
					overcoming obstacles.
				</li>
			</ul>

			<p>The user test covered these phases of product experience:</p>
			<figure>
				<img src={srcUserJoruney} class="" alt="Illustrations of different number types" />
			</figure>

			<h2>Research insights</h2>
			<p>
				We found that only 3 out of the 10 participants successfully sent an SMS to themselves,
				which was below our expectations. Our goal was to achieve a 100% success rate, with each
				participant completing the process within 5 minutes. To understand the reasons behind this
				outcome, we examined the entire user journeys. I conducted a detailed analysis of the tests,
				measuring the time each participant spent on the main phases of the process:
			</p>

			<figure>
				<img src={srcTime} class="" alt="Illustrations of different number types" />
			</figure>
			<p>From this analysis, the primary issues detected during the process were:</p>
			<h3>Difficult to find the right section in documentation</h3>
			<p>
				Some participants struggled to find the correct section in our documentation, with two
				spending 16 and 25 minutes respectively. This difficulty was primarily due to broken links
				on the platform, making it challenging for them to navigate to the appropriate section. Once
				they found the right place, it only took them a couple of minutes to understand what they
				needed to do.
			</p>

			<figure>
				<img
					src={srcCurrentdesign}
					class="box-shadow rounded"
					alt="Gif showing all number types together in one section"
				/>
				<figcaption>Previous design of the "Getting started with Sinch SMS API"</figcaption>
			</figure>

			<h3>Difficult to find the parameters in the platform</h3>
			<p>
				To use the Sinch SMS API, participants needed to locate three parameters: 1) their API
				token, 2) Service Plan ID, and 3) the Sinch test number provided for the trial. Most
				participants used links from the documentation to find them. However, they encountered
				several challenges in the process and still struggled to navigate the platform to find these
				three parameters. It took, on average, 6-8 minutes for the participants to locate them.
			</p>

			<figure>
				<video controls src={srcVideo} alt="Video showing the final product" muted>
					<track kind="captions" />
				</video>
				<figcaption class="xxs light">
					A participant explains the struggle to locate parameters
				</figcaption>
			</figure>

			<h3>Lack of error handling</h3>
			<p>
				Due to fraud attacks on our platform, some regions are temporarily restricted from sending
				SMS. Unfortunately, this means users in these regions aren't able to try the SMS API either.
			</p>

			<p>
				During the user test, UK numbers were blocked but there was no notification about this
				restriction. Participants simply didn't receive an SMS. They were not informed about their
				region being blocked. This created uncertainty about their verified phone numbers, leading
				some to think they had entered the wrong number upon registration.
			</p>

			<p>
				As a result, participants tried to verify and change the "TO" number, which led to another
				error. The API responded with "Messages can only be sent to your verified number in test
				mode." Users didn't understand what "in test mode" meant. This lack of clear communication
				and transparency breaks trust. Participants felt uncertain and frustrated, doubting the
				reliability of the platform. They questioned whether their actions were correct and whether
				the service was dependable. This eroded their confidence in the API and in the platform as a
				whole, making them less likely to trust and use the service in the future.
			</p>

			<figure>
				<img
					src={srcError}
					class="box-shadow rounded"
					alt="Gif showing all number types together in one section"
				/>
				<figcaption>
					An improved suggestion would be: "In test mode, the SMS API only sends messages to
					verified phone numbers. This ensures security. Verify your number in the Sinch Customer
					Dashboard."
				</figcaption>
			</figure>

			<div class="divider">
				<img src={srcDivider} alt="Divider svg" />
			</div>
			<h2 class="m" id="Part2">
				Part II: How might we ensure all participants are successful in sending a test SMS within 5
				minutes?
			</h2>
			<p>
				Ensuring all participants can build an app and send a test SMS within 5 minutes is vital. It
				shows the Sinch SMS API is easy and reliable, creating a strong first impression. Developers
				have low motivation at the start and need quick proof that it works. If it fails, they will
				quickly abandon it. A smooth first experience builds trust, leading to more conversions.
			</p>

			<figure>
				<img src={srcMotivation} class="" alt="Illustration showing why developers drop off" />
			</figure>

			<h3>Benchmarking & setting goals</h3>
			<p>
				I conducted a competitor analysis to compare our onboarding experience with that of our main
				competitors. This involved benchmarking their onboarding processes against ours, focusing on
				key aspects such as ease of use, clarity of instructions, speed of completion, and overall
				user satisfaction. By examining how competitors structured their onboarding journeys, what
				support materials they provided, and how they guided new users, we gained valuable insights
				into industry best practices.
			</p>

			<figure>
				<img src={srcCompetitorresearch} class="" alt="" />
				<figcaption>Example of a competitor's onboarding process</figcaption>
			</figure>

			<p>
				The goal was to understand how our experience measures up, recognizing that developers often
				evaluate multiple providers before making a decision. This comparative analysis highlighted
				our strengths and pinpointed areas where we lagged behind. It helped identify specific
				improvements we could make to streamline our process, reduce friction, and enhance the
				overall user experience. Leveraging these insights allowed us to align our onboarding
				process more closely with industry standards and best practices, ultimately making it more
				competitive and appealing to developers.
			</p>
			<figure>
				<img src={srcCompetitors} class="" alt="" />
				<figcaption>Comparison of competitors</figcaption>
			</figure>

			<p>
				Fueled by insights from competitor research and user tests, we set clear goals to address
				the biggest challenges in our onboarding process. Our primary objective was to remove
				roadblocks and ensure a smooth experience for developers. We systematically tackled these
				issues by working in fast iterations, focusing on eliminating friction and optimizing the
				onboarding funnel, and optimize the onboarding funnel for a smoother and more
				developer-friendly experience.
			</p>

			<h3>Goal 1: Reduce API Errors & help users solve them if they occur</h3>
			<p>
				To ensure the API was stable and reliable, we closely monitored logs and user feedback to
				identify and fix recurring issues.
			</p>

			<h4>Help users solve errors</h4>
			<p>
				Users lacked sufficient information about issues, so we added a link to our analytics tool,
				Message Search, when the API request was sent. Message Search provides detailed SMS logs,
				including error code descriptions, timestamps, delivery status, and fees. This allows users
				to understand and resolve issues related to the API request and increases the
				discoverability of Message Search. Long term, we plan to display this data directly in the
				UI on this page, but that is a later milestone.
			</p>

			<p>
				Additionally, we added the API response directly in the UI because we noticed some
				participants were using the browser console to view it. This change ensures users can easily
				access important information without resorting to technical workarounds.
			</p>
			<figure>
				<img
					src={srcAPIresponse}
					class=""
					alt="Illustration showing different parameters together"
				/>
			</figure>

			<h3>Goal 2: Reduce time to find parameters</h3>
			<p>
				Users were spending too much time searching for parameters, hindering the overall efficiency
				of their journey. They needed to navigate through multiple sections to retrieve them, often
				getting lost in the process. To address this, we aimed to keep them on the same page by
				consolidating all necessary parameters in one location.
			</p>
			<figure>
				<img
					src={srcParameters}
					class=""
					alt="Illustration showing different parameters together"
				/>
			</figure>

			<h3>Goal 3: Shorten time to find right section in documentation</h3>
			<p>
				To reduce the risk of having users struggle to find the right section in the documentation,
				we reviewed all critical links in the documentation and platform to ensure they functioned
				properly. We collaborated closely with the documentation team, suggesting improvements to
				help users find the right sections more quickly.
			</p>

			<p>
				We also introduced a dropdown with all SDKs and Rest API guides available. This was to help
				users faster find the most suitable section in the documentation.
			</p>

			<figure>
				<img
					src={srcSelectlanguage}
					class="box-shadow rounded"
					alt="Gif showing the possibility to switch between languages"
				/>
				<figcaption>
					Users can now select their preferred language to access documentation
				</figcaption>
			</figure>

			<h3>Goal 4: Prevent errors</h3>
			<p>
				Users testing the SMS API can only send messages to phone numbers verified on their account
				to prevent fraud and ensure platform security. Previously, the input field allowed users to
				type in numbers, causing errors when unverified numbers were entered. To reduce these errors
				and improve user experience, we replaced the input field with a dropdown menu of verified
				numbers.
			</p>

			<p>
				We also added the functionality to verify a new number directly on this page, eliminating
				the need for users to navigate to another page which was the case before.
			</p>

			<figure>
				<img src={srcInput} class="" alt="Illustration showing different parameters together" />
			</figure>

			<div class="divider">
				<img src={srcDivider} alt="Divider svg" />
			</div>

			<h2 class="m" id="Result">Result</h2>
			<p>
				The goal of this project was to optimize the onboarding journey for new developers testing
				the SMS API using an agile approach. We identified numerous user pain points and tracked the
				time it took for users to try the SMS API, aiming to reduce this time to under 5 minutes. My
				team and I enhanced the UI of the SMS Getting Started page and collaborated with other teams
				to improve the backend, API functionality, documentation, and test number provisioning.
			</p>

			<figure>
				<img src={srcOptimalJourney} class="" alt="" />
				<figcaption>
					Our goal was to streamline the SMS API onboarding, reducing completion time to under 5
					minutes
				</figcaption>
			</figure>

			<p>
				This ongoing project will be evaluated by usability tests in August 2024. However, we have
				already observed a surge in conversion rates and other metrics such as increased user
				satisfaction, reduced onboarding time, and higher engagement levels.
			</p>

			<p>
				Looking ahead, we will continue optimizing the SMS onboarding journey. Our focus will expand
				to cover more steps of the product adoption journey, including introducing messaging logs
				and providing better guidance on selecting phone numbers for sending live messages.
			</p>

			<figure>
				<img src={srcNewPage} class="box-shadow rounded" alt="" />
				<figcaption>
					Current design of the SMS Getting started page after the improvements
				</figcaption>
			</figure>

			<div class="infobox rounded" id="About-Sinch">
				<p>About Sinch</p>
				<p>
					Sinch provides communication APIs and applications for smooth interaction between
					companies and their customers. Their solutions cover diverse communication channels
					including SMS, voice, video, and social media platforms. This enables businesses to
					effectively engage with their audience across multiple platforms and devices, ensuring
					enhanced connectivity and customer satisfaction. <a href="https://www.sinch.com/"
						>Learn more about Sinch.</a
					>
				</p>
			</div>
		</div>

		<div class="sidebar">
			<div class="navigation rounded box-shadow blur">
				<p>Table of contents</p>
				<ul>
					<li><a href="#Part1">Part I: Current onboarding experience</a></li>
					<li>
						<a href="#Part2"
							>Part II: How might we ensure all participants are successful in sending a test SMS
							within 5 minutes?
						</a>
					</li>
					<li><a href="#Result">Result</a></li>
					<li><a href="#About-Sinch">About Sinch</a></li>
				</ul>
			</div>
		</div>
	</div>
</section>

<style>
</style>
