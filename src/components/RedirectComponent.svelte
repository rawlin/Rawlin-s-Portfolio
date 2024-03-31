<script>
	export let redirectName = 'Redirect';
	export let redirectLink = 'https://www.google.com';

    function handleClick() {
        window.open(redirectLink, '_blank', 'noopener,noreferrer')
    }
</script>

<div class="container" on:click={handleClick}>
	<p>{redirectName}</p>
	<svg class="icon"
		xmlns="http://www.w3.org/2000/svg"
		width="1em"
		height="1em"
		viewBox="0 0 24 24"
		{...$$props}
	>
		<path
			fill="currentColor"
			d="m16 8.4l-8.9 8.9q-.275.275-.7.275t-.7-.275q-.275-.275-.275-.7t.275-.7L14.6 7H7q-.425 0-.712-.288T6 6q0-.425.288-.712T7 5h10q.425 0 .713.288T18 6v10q0 .425-.288.713T17 17q-.425 0-.712-.288T16 16z"
		/>
	</svg>
</div>

<style>
	.container {
		display: flex;
		align-items: center;
		cursor: pointer;
	}

	.icon {
		transition: transform 0.3s ease;
		margin-left: 4px;
	}

	.container:hover .icon {
		transform: translate(0.2em, -0.2em);
	}

    .container.fill-div {
        display: block;
        height: 100%;
        width: 100%;
        text-decoration: none;
    }
</style>
