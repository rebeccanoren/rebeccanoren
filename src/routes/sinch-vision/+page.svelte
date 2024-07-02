<script context="module">

	import { Lightbox } from 'svelte-lightbox';
</script>

<script>
	let srcNumbertypes = '/sinch/vision/numbertypes.png';

	let numbertypes = {
  img: '/sinch/vision/numbertypes.png',
  imgMobile:  '/sinch/vision/numbertypes-small.png',
  desc: 'Different number type for SMS',
};

	let journey = {
  img: '/sinch/vision/user-journey.png',
  imgMobile:  '/sinch/vision/user-journey-small.png',
  desc: 'The steps to buy a local US number (also called 10DLC)',
};
	let srcQuotes = '/sinch/vision/quotes.svg';
	let srcCurrentOverivew = '/sinch/vision/current-overview.png';
	let srcCompareNumbers = '/sinch/vision/compare-numbers.gif';
	let srcNumbersOverview = '/sinch/vision/numbers-overview.gif';
	let srcNumberDetails = '/sinch/vision/number-details.png';
	let srcBrandProfile = '/sinch/vision/brand-profile.svg';

	let srcDivider = 'divider.svg';

	let srcSinchOnboarding = '/sinch/onboarding/onboarding.svg';
	let enter1 = false;
</script>

<svelte:head>
	<title>Defining the vision for numbers & senders</title>
	<meta
		name="description"
		content="UX Case Study: How might we simplify the process to buy numbers with Sinch?"
	/>
</svelte:head>

<section class="case">
	<div class="container">
		<div class="description">
			<p class="xs">Sinch (2024)</p>
			<h1 class="xl">Defining the vision for numbers & senders</h1>
			<p class="s">
				Sinch offers a large selection of phone numbers worldwide, essential for using our SMS API.
				However, the separate management of these numbers by different internal teams has led to a
				fragmented and inconsistent user experience.
			</p>

			<div class="summary rounded">
				<p>Summary</p>
				<p>
					As the UX Design Lead, I am working to make it easier for users to buy numbers and senders
					on our platform. I am collaborating with stakeholders using an iterative approach to
					explore and gather feedback on the vision. This is an ongoing project.
				</p>
			</div>

			<h2 class="m" id="Part1">Part I: Understanding the current state</h2>
			<p>
				To use the SMS API, you must have a phone number. Different markets and number types, such
				as 10DLC, Toll-free, Short Codes, and Alphanumeric Sender IDs, each come with their own
				specific regulations and requirements. This complexity makes it challenging for users to
				understand which type of number they need and how to comply with the various regulations in
				different regions.
			</p>


			<div class="lightbox">
				<Lightbox description={numbertypes.desc}>
					<picture>
						<source srcset={numbertypes.imgMobile} media="(max-width: 600px)">
						<source srcset={numbertypes.img} media="(min-width: 601px)">
						<img src={numbertypes.img} alt={numbertypes.desc}>
					  </picture>
			</Lightbox>
			<p class="image-description">{numbertypes.desc}</p>
		</div>



			<p>
				This project started with a deep dive into research, blending stakeholder and user
				interviews, benchmarking, and synthesizing prior studies. From this, I uncovered key
				insights. To be mindful of your time, this case study will focus on the two most important
				findings:
			</p>

			<h3>Customers have a hard time understanding how messaging works</h3>
			<p>
				New and existing customers face a significant knowledge gap, particularly with
				telecom-related concepts. They struggle to understand which numbers or senders they should
				use for their specific needs, and the platform isn't providing them with sufficient
				guidance.
			</p>


			<div class="lightbox">
				<Lightbox description={journey.desc}>
					<picture>
						<source srcset={journey.imgMobile} media="(max-width: 600px)">
						<source srcset={journey.img} media="(min-width: 601px)">
						<img src={journey.img} alt={journey.desc}>
					  </picture>
			</Lightbox>
			<p class="image-description">{journey.desc}</p>
		</div>

		
		

			<h3>Poor navigation & broken journeys</h3>
			<p>
				Users need to navigate through multiple sections of the platform and provide detailed
				information about the company sending the SMS and how users consent to receive messages. The
				process doesn't feel seamless or intuitive. Even users who understand the steps struggle to
				find the right sections within the platform, making the experience frustrating and
				inefficient.
			</p>

			<figure>
				<img src={srcQuotes} class="" alt="Illustrating the journey to buy a 10DLC number" />
			</figure>

			<p>
				Additionally, customers often contact account managers with questions about purchasing phone
				numbers consuming significant time. This distraction prevents them from focusing on
				strategic activities like developing client relationships, optimizing campaigns, and
				addressing complex customer needs.
			</p>

			<div class="divider">
				<img src={srcDivider} alt="Divider svg" />
			</div>
			<h2 class="m" id="Part2">
				Part II: How might we simplify the process to buy numbers with Sinch?
			</h2>

			<p>
				With the key research insights in mind, I began envisioning an improved journey to buy
				numbers. I sketched a high-level user journey focusing on the following key phases: finding
				the right number, understanding market regulations, buying the number, and getting approval
				to send SMS. Then, I prototyped various approaches to streamline and enhance this process.
				Please note that this work is still in progress, and the following designs are preliminary
				sketches, not final UI.
			</p>

			<h3>Goal 1: Centralized section for numbers & senders</h3>
			<p>
				After re-evaluating the current structure, I proposed a new information architecture to
				enhance the user experience. Currently, numbers and senders are scattered across multiple
				sections, making it difficult to get a comprehensive overview. By centralizing them in one
				section, users can easily manage all their numbers and senders within their account.
			</p>

			<figure>
				<img
					src={srcNumbersOverview}
					class="box-shadow rounded"
					alt="All number types together in one section"
				/>
				<figcaption>All numbers and senders together</figcaption>
			</figure>

			<h3>Goal 2: Simplifying complex telecom terminology</h3>
			<p>
				If you're a telecom pro, terms like 10DLC, Campaigns, and Alphanumeric Sender ID might be
				second nature. For the rest of us, they're a bit of a head-scratcher.
			</p>

			<figure>
				<img
					src={srcCurrentOverivew}
					class="box-shadow rounded"
					alt="Screenshot of current overview page for numbers"
				/>
				<figcaption>
					The current overview page doesn't effectively guide users in understanding what number
					type they need or explains the steps
				</figcaption>
			</figure>

			<p>
				To simplify these terms, I proposed using interactive tables for comparing number types and
				their capabilities, adding visual illustrations for clarity, and incorporating interactive
				guides that mimic the questions account managers ask. This approach aims to help customers
				easily find the perfect number type. Choosing the right number type depends on factors like
				the target country, message type (marketing, verification, alerts) and whether recipients
				need to reply.
			</p>
			<figure>
				<img
					src={srcCompareNumbers}
					class="box-shadow rounded"
					alt="Gif showing a table with all numbers types per region"
				/>
				<figcaption>
					Enable users to view and compare available numbers in different markets
				</figcaption>
			</figure>

			<h3>Goal 3: Smoother process to register numbers</h3>
			<p>
				In telecom terms, a "campaign" means registering a number with operators. Operators need to
				know: 1) who is sending the messages and 2) what messages will be sent. This information is
				crucial for regulatory compliance and spam prevention. By using clear labels and
				step-by-step instructions, users can easily see if their number is ready to use and
				understand the actions they need to take.
			</p>

			<figure>
				<img
					src={srcNumberDetails}
					class="box-shadow rounded"
					alt="Gif showing a table with all numbers types per region"
				/>
				<figcaption>
					My suggestion: Outline the steps required for registration in the detailed page for a
					phone number
				</figcaption>
			</figure>

			<h3>Goal 4: Streamline information collection</h3>
			<p>
				Operators often ask for the same details about companies. Currently, customers must enter
				this information separately for each request, which is frustrating and time-consuming. To
				make things easier, we need to align the information collection processes. By creating a
				centralized "Brand Profile," we can store all this information in one place. This means that
				once a customer sets up their Brand Profile, they won't need to re-enter their details for
				each new request.
			</p>

			<figure>
				<img
					src={srcBrandProfile}
					class=""
					alt="GIF showing a table with all numbers types per region"
				/>
			</figure>

			<div class="divider">
				<img src={srcDivider} alt="Divider svg" />
			</div>

			<h2 class="m" id="Result">Result</h2>
			<p>
				The goal of this project is to define a shared vision of how we want the user experience for
				buying numbers to be. This vision will foster cohesion and synergy across multiple teams
				within our organization through an iterative and collaborative process. It will guide us in
				making informed decisions that align with our larger goals throughout the research and
				design exploration. I've identified several key priorities:
			</p>

			<ul class="margin">
				<li>Optimize information architecture to support a smoother user journey.</li>
				<li>
					Bridge the knowledge gap by explaining the different types of phone numbers across various
					markets, and what users need to know about each type.
				</li>
				<li>
					Streamline information registration processes using reusable brand profiles for
					efficiency.
				</li>
			</ul>

			<p>To experience this firsthand, you can try out the prototype below.</p>

			<iframe title="figma"
				style="border: 1px solid rgba(0, 0, 0, 0.1);"
				width="800"
				height="450"
				src="https://www.figma.com/embed?embed_host=share&url=https%3A%2F%2Fwww.figma.com%2Fproto%2FXkUn58KXLZXp3gQt9uCWWG%2FUX-Future-Vision%3Fpage-id%3D2056%253A32544%26node-id%3D5354-66826%26viewport%3D-6126%252C7273%252C0.28%26t%3DkC49SuiONW905Lo0-1%26scaling%3Dscale-down%26content-scaling%3Dfixed%26starting-point-node-id%3D5354%253A66826%26show-proto-sidebar%3D1"
				allowfullscreen
			/>

			<h2 class="s">Next steps</h2>
			<p>
				Currently, we're at the early stages of this initiative; focusing on research, design
				exploration, and gathering feedback from stakeholders. Looking ahead, we'll also consider
				the needs of customers buying numbers for Voice APIs. These customers often require numbers
				in batch. Unlike SMS numbers, getting Voice numbers usually doesn't involve as much
				registration.
			</p>

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

			<div class="divider">
				<img src={srcDivider} alt="Divider svg" />
			</div>

			<div class="next-case">
				<h3>Next up</h3>
				<a data-sveltekit-prefetch href="/sinch-getting-started">
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
					<li><a href="#Part1">Part I: Understanding the current state </a></li>
					<li>
						<a href="#Part2"
							>Part II: How might we simplify the process to buy numbers with Sinch?
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
