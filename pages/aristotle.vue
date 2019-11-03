<template lang="pug">
sui-container(text text-align='center' style="padding-top: 125px")
	.ui.huge.header.dignity A Bugger For The Bottle
	.ui.large.header.with.dignity Aristotle Aristotle
	img(src='/biohazard.svg', width='150px' style="margin-top: 25px;")

	.ui.icon.warning.message
		i.material-icons.md-48 rowing
		.content
			.ui.left.aligned.header.dignity Have You Heard The Word?
			p(style="text-align: left;") Νε vελ ομνεσ φαβθλασ. Cορπορα cοπιοσαε? Νε vελ ομνεσ φαβθλασ! Cορπορα cοπιοσαε!
	.ui.hidden.divider

	div
		sui-button.dignity(primary='')
			i.material-icons mic
			|  Shall Be First
		sui-button.dignity(secondary='')
			i.material-icons settings_power
			|  Shall Be Last

		button.ui.large.disabled.negative.icon.button.with.dignity
			i.chess.icon
			| &nbsp;Middling Ages

	sui-divider
	sui-grid(:columns='3', divided='', stackable='true')
		sui-grid-row(stretched='')
			sui-grid-column
				sui-segment
					i.material-icons waves
					|  Fungo Mungo
			sui-grid-column
				sui-segment
					i.material-icons local_library
					|  Fungo Mungo
				sui-segment
					i.material-icons directions_bike
					|  Fungo Mungo
			sui-grid-column
				sui-segment
					i.material-icons beach_access
					|  Fungo Mungo
				sui-segment
					i.material-icons settings_power
					|  Fungo Mungo
				sui-segment
					i.material-icons settings_input_antenna
					|  Fungo Mungo
</template>

<script>
import AppLogo from '~/components/AppLogo.vue'

export default {
	components: {
		AppLogo
	}
}
</script>

<script>
export default {
	head () {
		return {
			script: [
				{ src: 'https://cdnjs.cloudflare.com/ajax/libs/jquery/3.1.1/jquery.min.js' },
				{ src: 'https://cdn.jsdelivr.net/npm/semantic-ui@2.4.0/dist/semantic.min.js' }
			],
			link: [
				{ rel: 'stylesheet', href: 'https://fonts.googleapis.com/css?family=News+Cycle|Material+Icons' },
				{ rel: 'stylesheet', href: 'https://cdn.jsdelivr.net/npm/semantic-ui@2.4.0/dist/semantic.min.css' }
			]
		}
	}
}
</script>

<style lang="scss">
.container {
	text-align: center;
	min-height: 100vh;
	padding: 40px;
}

.material-icons, .fa {
	vertical-align: middle;
}
.dignity {
	font-family: 'News Cycle', sans-serif !important;
	font-weight: 300 !important;
}
</style>
