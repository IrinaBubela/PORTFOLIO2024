<script>
	import "../app.scss";
	import Navbar from "$lib/Navbar.svelte";

	const links = [
		{ name: "Home", href: "/" },
		{ name: "About Me", href: "#about-me" },
		{ name: "Projects", href: "#projects" },
		{ name: "Experience", href: "#experience" },
	];
</script>

<Navbar {links}></Navbar>

<main class="flex flex-col items-center p-6 pt-20">
	<slot></slot>

	<div style="opacity: 1; transform: none;" class="socials">
		<ul>
			<li>
				<a
					href="https://github.com/IrinaBubela"
					target="_blank"
					rel="noopener noreferrer"
				>
					<svg
						xmlns="http://www.w3.org/2000/svg"
						viewBox="0 0 24 24"
						width="24"
						height="24"
						><path fill="none" d="M0 0h24v24H0z"></path><path
							d="M12 2C6.475 2 2 6.475 2 12a9.994 9.994 0 0 0 6.838 9.488c.5.087.687-.213.687-.476 0-.237-.013-1.024-.013-1.862-2.512.463-3.162-.612-3.362-1.175-.113-.288-.6-1.175-1.025-1.413-.35-.187-.85-.65-.013-.662.788-.013 1.35.725 1.538 1.025.9 1.512 2.338 1.087 2.912.825.088-.65.35-1.087.638-1.337-2.225-.25-4.55-1.113-4.55-4.938 0-1.088.387-1.987 1.025-2.688-.1-.25-.45-1.275.1-2.65 0 0 .837-.262 2.75 1.026a9.28 9.28 0 0 1 2.5-.338c.85 0 1.7.112 2.5.337 1.912-1.3 2.75-1.024 2.75-1.024.55 1.375.2 2.4.1 2.65.637.7 1.025 1.587 1.025 2.687 0 3.838-2.337 4.688-4.562 4.938.362.312.675.912.675 1.85 0 1.337-.013 2.412-.013 2.75 0 .262.188.574.688.474A10.016 10.016 0 0 0 22 12c0-5.525-4.475-10-10-10z"
						></path></svg
					></a
				>
			</li>
			<li>
				<a
					href="https://www.linkedin.com/in/iryna-bubela-17259a1a2/"
					target="_blank"
					rel="noopener noreferrer"
					><svg
						xmlns="http://www.w3.org/2000/svg"
						viewBox="0 0 24 24"
						width="24"
						height="24"
						><path fill="none" d="M0 0h24v24H0z"></path><path
							d="M6.94 5a2 2 0 1 1-4-.002 2 2 0 0 1 4 .002zM7 8.48H3V21h4V8.48zm6.32 0H9.34V21h3.94v-6.57c0-3.66 4.77-4 4.77 0V21H22v-7.93c0-6.17-7.06-5.94-8.72-2.91l.04-1.68z"
						></path></svg
					></a
				>
			</li>
		</ul>
		<div class="line"></div>
	</div>
</main>

<style lang="scss">
	@import "../app.scss";

	.socials {
		align-items: center;
		bottom: 0;
		display: flex;
		flex-direction: column;
		position: fixed;
		right: 30px;
		z-index: 3;
		ul li {
			margin: 0 0 10px;
		}
	}

	.socials ul li {
		margin: 0 0 10px;

		a {
			align-items: center;
			background-color: #fff;
			border-radius: 50%;
			display: block;
			display: flex;
			font-size: 0;
			height: 25px;
			justify-content: center;
			transition: all 0.2s ease;
			width: 25px;
		}
		svg {
			width: 15px;
		}
	}
	
	.line {
		background-color: #3e3552;
		height: 90px;
		width: 1px;
	}
</style>
