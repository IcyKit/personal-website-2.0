<section class="about">
	<h2>About me</h2>
	<div class="about-container">
		<div class="image">
			<img src="profile2.jpg" alt="profile photo" />
		</div>
		<p>
			I'm a 20 year old Fullstack Developer from St. Petersburg, Russia.I have 1 year of hands-on
			experience designing, developing, and implementing applications and solutions using a range of
			technologies and programming languages.Previously, I was an Affiliate Manager and UI/UX
			Designer. Such different areas of IT gave me a complete understanding of the creation of the
			product and a view from each side of the development.
		</p>
	</div>
</section>

<style>
	.about {
		padding-top: 100px;
	}

	h2 {
		font-size: 22px;
		font-weight: 500;
		margin-bottom: 30px;
	}

	.about-container {
		display: grid;
		justify-items: stretch;
		align-items: center;
		grid-template-columns: 1fr 1fr;
		gap: 50px;
	}

	p {
		font-size: 16px;
		font-weight: 300;
		line-height: 24px;
	}

	img {
		border-radius: 30px;
	}

	@media (max-width: 670px) {
		.about {
			padding-top: 50px;
		}

		.about-container {
			grid-template-columns: 1fr;
			gap: 20px;
		}

		h2 {
			margin-bottom: 20px;
		}

		.image {
			order: 2;
		}

		img {
			height: 400px;
			width: 100%;
			object-fit: cover;
		}
	}

	@media (max-width: 460px) {
		h2 {
			font-size: 18px;
		}
	}

	@media (max-width: 425px) {
		img {
			height: 230px;
		}
	}
</style>
