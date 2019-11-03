<template lang="pug">
sui-container(text text-align='center' style="padding-top: 125px")
	.ui.huge.header.dignity O Hell! O Ease!
	.ui.medium.header.with.dignity(style="margin-top: 25px;") Abelard &amp; Heloise &amp; Amor a lo Divino
	.ui.hidden.divider

	img(src='/alchemy-sulphuric.svg', width='125px')

	.ui.icon.small.warning.message
		i.huge.at.icon
		.content
			.ui.left.aligned.header.with.dignity Rhetorician Makes Admission
			p(style="text-align: left;") Νε vελ ομνεσ φαβθλασ. Cορπορα cοπιοσαε! Cορπορα cοπιοσαε! Cορπορα cοπιοσαε? φαβθλασ.
	.ui.hidden.divider

	div
		sui-button.dignity(primary='', style="padding: 12px")
			i.material-icons mic
			|  Medieval
		sui-button.dignity(secondary='', style="padding: 12px")
			i.material-icons settings_power
			|  Primeval

	sui-hidden-divider
	sui-divider
	sui-grid(:columns='3', divided='', stackable='')
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
