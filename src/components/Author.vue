<template>
	<div class="author">

		<g-image alt="Author image" class="author__image" src="https://cdn.discordapp.com/avatars/713632188863610911/00d4f89c959edd860c86645e494048ba.jpeg" width="180" height="180" blur="5" />

		<h1 v-if="showTitle" class="author__site-title">
			{{ $static.metadata.siteName }}
		</h1>

		<p class="author__intro">
		    Hey My name is Maxim King, I'm a backend developer and work on some pretty cool projects. This is my personal blog enjoy!
		</p>

		<p class="author__links">
			<a href="//twitter.com/MaximKing8">Follow My Twitter</a>
			<a href="//github.com/MaximKing1">GitHub</a>
		</p>

	</div>
</template>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>

<script>
export default {
	props: ['showTitle']
}
</script>

<style lang="scss">
.author {
	margin: 0 auto;
	max-width: 500px;
	text-align: center;
	padding: calc(var(--space) / 2) 0;

	&__image {
		border-radius: 100%;
		width: 90px;
		height: 90px;
		margin-bottom: 1em;
	}

	&__intro {
		opacity: .8;
	}

	&__site-title {
		font-size: 1.5em;
	}

	&__links {
		margin-top: -.5em;
		a {
			margin: 0 .5em;
		}
	}
}
</style>
