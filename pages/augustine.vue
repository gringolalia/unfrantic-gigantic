<template lang="pug">
sui-container(text text-align='center' style="padding-top: 125px")
	.ui.huge.header.dignity Saint Augustine
	.ui.large.header.with.dignity I Dreamed I Saw Joe Hill Last Night
	.ui.hidden.divider
	img(src='/alchemy-sulphuric.svg', width='100px')

	.ui.icon.negative.message
		i.chess.king.icon
		.content
			.ui.left.aligned.header.with.dignity Bishop of Hippopotami
			.ui.hidden.divider
			.ui.left.aligned.tiny.header.with.dignity Μνεσαρcηθμ cοτιδιεqθε αδ μελ. Μεα νατθμ ινvιδθντ ατ. Ετ vιμ μελιθσ ελοqθεντιαμ. Τολλιτ σεντεντιαε ηισ νε, qθι ρεqθε διcαμ ταμqθαμ ιν, αφφερτ δισπθτανδο εθμ cθ.

	.ui.hidden.divider

	div
		sui-button.dignity(primary='',  style="margin: 12px")
			i.material-icons mic
			| &nbsp; Shall Be First
		sui-button.dignity(secondary='', style="margin: 12px")
			i.material-icons settings_power
			| &nbsp; Shall Be Last

	sui-divider
	sui-grid(:columns='3', divided='', stackable='')
		sui-grid-row(stretched='')
			sui-grid-column
				sui-segment
					i.material-icons waves
					| &nbsp; Fungo Mungo
			sui-grid-column
				sui-segment
					i.material-icons local_library
					| &nbsp; Fungo Mungo
				sui-segment
					i.material-icons directions_bike
					| &nbsp; Fungo Mungo
			sui-grid-column
				sui-segment
					i.material-icons beach_access
					| &nbsp; Fungo Mungo
				sui-segment
					i.material-icons settings_power
					| &nbsp; Fungo Mungo
				sui-segment
					i.material-icons settings_input_antenna
					| &nbsp; Fungo Mungo
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
