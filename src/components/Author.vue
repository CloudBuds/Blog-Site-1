<template>
	<div class="author">

		<g-image alt="Author image" class="author__image" src="~/assets/images/981E4386-8142-463C-BF35-CEA796AB6C2E.jpeg" width="180" height="180" blur="5" />

		<h1 v-if="showTitle" class="author__site-title">
			{{ $static.metadata.siteName }}
		</h1>

		<p class="author__intro">
			Infinity Bot List is The future of Discord Bot Listing Services, we make it easier for you to advertise and grow your bots.
		</p>

		<p class="author__links">
			<a href="//twitter.com/InfinityBotList">Follow us on Twitter</a>
			<a href="//github.com/InfinityBotList">GitHub</a>
                        <a href="//infinitybotlist.com/discord">Discord</a>
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
