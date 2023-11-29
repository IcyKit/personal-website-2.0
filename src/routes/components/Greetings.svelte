<div class="head">
	<div>
		<h2><span>Hi!</span></h2>
		<h2>My name is <span>Nikita Efimov</span></h2>
		<p>Fullstack Developer from Saint Petersburg, Russia</p>
	</div>
	<div class="avatar">
		<img src="profile.png" alt="profile photo" />
	</div>
</div>

<style>
	.head {
		padding-top: 100px;
		display: flex;
		align-items: center;
		justify-content: space-between;
		flex-wrap: wrap;
	}

	h2 {
		font-size: 28px;
		line-height: 36px;
	}

	span {
		font-weight: bold;
	}

	p {
		font-size: 16px;
		padding-top: 10px;
	}

	img {
		width: 220px;
		height: 220px;
		border-radius: 30px;
	}

	@media (max-width: 650px) {
		p {
			max-width: 190px;
		}

		h2 {
			max-width: 200px;
		}
	}

	@media (max-width: 460px) {
		.head {
			padding-top: 50px;
		}

		h2 {
			font-size: 22px;
			line-height: 28px;
			max-width: 300px;
		}
		p {
			max-width: 200px;
			font-size: 14px;
			margin-bottom: 20px;
			padding-top: 5px;
		}

		.avatar {
			width: 100%;
		}

		img {
			object-fit: cover;
			width: 100%;
		}
	}
</style>
