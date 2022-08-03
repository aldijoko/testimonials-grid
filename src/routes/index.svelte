<script>
</script>

<div class="container">
	<div class="card cardOne">
		<img src="images/image-daniel.jpg" alt="Daniel" class="card__img accent-border" />
		<h2 class="card__name">Daniel Clifford</h2>
		<p class="card__title">Verified Graduate</p>
		<p class="card__main-quote">
			I received a job offer mid-course, and the subjects I learned were current, if not more so, in
			the company I joined. I honestly feel I got every penny’s worth.
		</p>
		<p class="card__testimonial">
			“ I was an EMT for many years before I joined the bootcamp. I’ve been looking to make a
			transition and have heard some people who had an amazing experience here. I signed up for the
			free intro course and found it incredibly fun! I enrolled shortly thereafter. The next 12
			weeks was the best - and most grueling - time of my life. Since completing the course, I’ve
			successfully switched careers, working as a Software Engineer at a VR startup. ”
		</p>
	</div>
	<div class="card cardTwo">
		<img src="images/image-jonathan.jpg" alt="Jonathan" class="card__img" />
		<h2 class="card__name">Jonathan Walters</h2>
		<p class="card__title">Verified Graduate</p>
		<p class="card__main-quote">The team was very supportive and kept me motivated</p>
		<p class="card__testimonial">
			“ I started as a total newbie with virtually no coding skills. I now work as a mobile engineer
			for a big company. This was one of the best investments I’ve made in myself. ”
		</p>
	</div>
	<div class="card cardThree">
		<img src="images/image-jeanette.jpg" alt="Jeanette" class="card__img" />
		<h2 class="card__name">Jeanette Harmon</h2>
		<p class="card__title">Verified Graduate</p>
		<p class="card__main-quote">An overall wonderful and rewarding experience</p>
		<p class="card__testimonial">
			“ Thank you for the wonderful experience! I now have a job I really enjoy, and make a good
			living while doing something I love. ”
		</p>
	</div>

	<div class="card cardFour">
		<img src="images/image-patrick.jpg" alt="Patrick" class="card__img accent-border" />
		<h2 class="card__name">Patrick Abrams</h2>
		<p class="card__title">Verified Graduate</p>
		<p class="card__main-quote">
			Awesome teaching support from TAs who did the bootcamp themselves. Getting guidance from them
			and learning from their experiences was easy.
		</p>
		<p class="card__testimonial">
			“ The staff seem genuinely concerned about my progress which I find really refreshing. The
			program gave me the confidence necessary to be able to go out in the world and present myself
			as a capable junior developer. The standard is above the rest. You will get the personal
			attention you need from an incredible community of smart and amazing people. ”
		</p>
	</div>

	<div class="card cardFive">
		<img src="images/image-kira.jpg" alt="Kira" class="card__img" />
		<h2 class="card__name">Kira Whittle</h2>
		<p class="card__title">Verified Graduate</p>
		<p class="card__main-quote">Such a life-changing experience. Highly recommended!</p>
		<p class="card__testimonial">
			“ Before joining the bootcamp, I’ve never written a line of code. I needed some structure from
			professionals who can help me learn programming step by step. I was encouraged to enroll by a
			former student of theirs who can only say wonderful things about the program. The entire
			curriculum and staff did not disappoint. They were very hands-on and I never had to wait long
			for assistance. The agile team project, in particular, was outstanding. It took my learning to
			the next level in a way that no tutorial could ever have. In fact, I’ve often referred to it
			during interviews as an example of my developent experience. It certainly helped me land a job
			as a full-stack developer after receiving multiple offers. 100% recommend! ”
		</p>
	</div>
</div>

<style>
	.container {
		display: flex;
		flex-direction: column;
		align-items: center;
		max-width: 1440px;
		margin: 0 auto;
	}

	.card {
		grid-area: card;
		box-sizing: border-box;
		background: #733fc8;
		border-radius: 10px;
		padding: 2em 1.75em;
		margin: 1em;
		display: grid;
		grid-template-columns: 45px auto;
		/* grid-template-rows: 16px 16px auto minmax(auto, 1fr); */
		grid-template-areas:
			'img name'
			'img title'
			'main-quote main-quote'
			'testimonial testimonial';
	}

	.cardOne {
		grid-area: cardOne;
		background-color: var(--violet);
		background-image: url('images/bg-pattern-quotation.svg');
		background-repeat: no-repeat;
		background-position: 85% 0%;
		/* padding: 50px; */
	}

	.cardTwo {
		grid-area: cardTwo;
		background-color: var(--darkGrayish);
	}

	.card__name {
		grid-area: name;
		font-size: 0.8125rem;
		font-weight: 500;
	}

	.card__title {
		grid-area: title;
		font-size: 0.6875rem;
		opacity: 50%;
		margin-top: 2px;
	}

	.card__main-quote {
		grid-area: main-quote;
		font-size: 1.25rem;
		font-weight: 600;
		margin: 1em 0;
	}

	.card__testimonial {
		font-size: 0.8125rem;
		grid-area: testimonial;
		color: var(--testimonial-color);
		opacity: 70%;
		line-height: 1.6;
	}

	.card__img {
		grid-area: img;
		height: 28px;
		width: auto;
		border-radius: 100%;
		margin-top: 2px;
	}

	.cardThree {
		grid-area: cardThree;
		background-color: var(--white);
		color: var(--darkGrayish);
	}

	.cardFour {
		grid-area: cardFour;
		background-color: var(--darkBlackish);
	}

	.cardFive {
		grid-area: cardFive;
		background-color: var(--white);
		color: var(--darkGrayish);
	}

	@media (min-width: 1024px) {
		/* multiple cards layout */
		.container {
        display: grid;
        grid-template-columns: minmax(250px, auto) minmax(250px, auto);
        grid-template-areas:
            "cardOne cardOne cardTwo cardFive"
            "cardThree cardFour cardFour cardFive";
        gap: 2em;
        padding: 3em;
        align-items: unset;
    }

    .card {
        margin: 0;
    }
	}
</style>
