<svelte:head>
	<title>Portfolio | Coming Soon</title>
	<meta
		name="description"
		content="Personal portfolio website currently under construction."
	/>
</svelte:head>

<script lang="ts">
    import avatar from "$lib/assets/ashley.png";
	const name = "Ashley";
</script>

<div class="background">
	<div class="card">
		<div class="avatar">
			<img src={avatar} alt="Profile Picture">
		</div>

		<h1>{name}</h1>
		<p class="subtitle">Animator • Roblox Developer</p>

		<div class="divider"></div>

		<h2>🚧 Under Construction</h2>
		<p class="description">
			I'm currently building something beautiful. My portfolio will be available soon.
			Check back later!
		</p>

		<button disabled>Coming Soon</button>
	</div>
</div>

<style>
	:global(body) {
		margin: 0;
		font-family:
			Inter,
			system-ui,
			-apple-system,
			BlinkMacSystemFont,
			"Segoe UI",
			sans-serif;
	}

	.background {
		min-height: 100vh;
		display: flex;
		align-items: center;
		justify-content: center;
		padding: 2rem;
		background:
			radial-gradient(circle at top, #ffd6e7, transparent 40%),
			linear-gradient(135deg, #fff7fb, #ffe9f3);
	}

	.card {
		width: min(450px, 100%);
		background: rgba(255, 255, 255, 0.8);
		backdrop-filter: blur(16px);
		border-radius: 24px;
		padding: 3rem;
		text-align: center;
		box-shadow: 0 20px 50px rgba(0, 0, 0, 0.08);
		border: 1px solid rgba(255, 255, 255, 0.6);
	}

    .avatar {
        width: 120px;
        height: 120px;
        margin: 0 auto 1.5rem;
        border-radius: 50%;
        overflow: hidden;
        border: 4px solid #ff8ec7;
        box-shadow: 0 8px 24px rgba(255, 142, 199, 0.3);
    }

    .avatar img {
        width: 100%;
        height: 100%;
        object-fit: cover;
        display: block;
    }

	h1 {
		margin: 0;
		font-size: 2.5rem;
		color: #222;
	}

	.subtitle {
		margin-top: 0.5rem;
		color: #666;
		font-size: 1rem;
	}

	.divider {
		width: 70px;
		height: 4px;
		border-radius: 999px;
		background: #ff8ec7;
		margin: 2rem auto;
	}

	h2 {
		margin: 0;
		color: #333;
		font-size: 1.5rem;
	}

	.description {
		margin-top: 1rem;
		color: #666;
		line-height: 1.7;
	}

	button {
		margin-top: 2rem;
		padding: 0.9rem 2rem;
		border: none;
		border-radius: 999px;
		background: #ff8ec7;
		color: white;
		font-size: 1rem;
		font-weight: 600;
		cursor: not-allowed;
		opacity: 0.9;
	}

	@media (max-width: 600px) {
		.card {
			padding: 2rem;
		}

		h1 {
			font-size: 2rem;
		}
	}
</style>