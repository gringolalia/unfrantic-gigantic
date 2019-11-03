<template lang="pug">
sui-container(text text-align='center' style="padding-top: 125px")
	.ui.huge.header.dignity Toulmin Had a Schema
	img(src='/alchemy-sulphuric.svg', height='100px')

	.ui.icon.warning.message
		i.lightbulb.outline.icon
		.content
			.header.with.dignity.left Another Bard of Harvard Yard
			p.left Νε vελ ομνεσ φαβθλασ. Cορπορα cοπιοσαε. Vιμ ωισι οφφενδιτ ρεφορμιδανσ τε, ατqθι νονθμυ πθτεντ νο qθι, vελ αδ ενιμ vερι φαλλι.
	.ui.hidden.divider

	div
		sui-button.monkey.dignity(primary='', data-title="Popcorn", data-content="An explanatory interruption to orient the user")
			i.material-icons mic
			| 	Syllogism
		sui-button.dignity(secondary='')
			i.material-icons settings_power
			|  Warrant
		sui-button.dignity(negative='')
			i.material-icons translate
			| Rebuttal

		.ui.button.with.dignity(data-tooltip="Ghostly messages to orient your user experience" data-position="top center" data-inverted="true")
			i.material-icons ring_volume
			| Andy Warhol


	sui-divider
	sui-grid(:columns='3', divided='')
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
$('sui-button')
  .popup()
;
</script>

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
