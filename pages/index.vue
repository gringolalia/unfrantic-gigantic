<template lang="pug">

sui-container(text text-align='center' style="padding-top: 125px")
	.ui.huge.header.dignity Nuxted Sin Taxes
	img(src='../static/alchemy-sulphuric.svg', width='125px' style="margin: 15px 15px")

	.ui.large.header.with.dignity(style="margin-top: 25px;") Rubricated Rhetoric
	.ui.medium.header.with.dignity(style="margin-top: 5px;") Ant Sanctum Index
	.ui.small.header.with.dignity(style="margin-top: 5px;"	) Semantic and Nuxt
	.ui.hidden.divider

	.ui.icon.warning.message
		i.sun.icon
		.content
			.ui.left.aligned.header.with.dignity Have You Heard The Word?
			p(style="text-align: left;") Νε vελ ομνεσ φαβθλασ. Cορπορα cοπιοσαε?  Μνεσαρcηθμ cοτιδιεqθε αδ μελ? Cορπορα cοπιοσαε!
	.ui.hidden.divider

	div
		sui-button.dignity(primary style="padding:12px;")
			i.material-icons mic
			|  Exordium
		sui-button.dignity(secondary style="padding:12px;")
			i.material-icons settings_power
			|  Peroration

		sui-button.with.dignity(warning @click.native='open = true')
			i.material-icons(style="margin-right: 8px") all_inclusive
			| Pi a la Modal



		sui-modal.with.dignity(animation='fade' v-model='open' size='tiny')
			sui-modal-header.with.dignity
				sui-icon(name="sun" size="large")
				| Cruzada Albigense

			sui-modal-content(image)
				sui-image(wrapped size='large' src='/alchemy-sulphuric.svg' width="150px")
				sui-modal-description
					sui-header.with.dignity Os Catharitos de Albi

					p Vιμ νο vολθπτθα αππελλαντθρ ρεπρεηενδθντ. Ατ δθισ απεριαμ vολθπταρια μεα. Ιδ αλιι δεβιτισ περφεcτο περ, vισ ετ δεcορε ορνατθσ σαλθτανδι. Νο φεθγιατ σινγθλισ λαβοραμθσ εοσ, εοσ μεντιτθμ παρτιενδο εξ, μει ιδqθε σενσεριτ αν.

			sui-modal-actions
				sui-button.with.dignity(primary @click.native='toggle')
					i.fas.fa-star-and-crescent.fa-2x
					| Divertir
				sui-button.with.dignity(secondary @click.native='toggle')
					i.fas.fa-sun.fa-2x
					| Aborrecer

		sui-divider
		sui-grid(:columns='3' divided  stackable)
			sui-grid-row(stretched)
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


	h1.gigantic.header(is='sui-header' icon text-align='center')
		i.fa.fa-mosque.fa-4x(circular)
		sui-header-content.huge.with.dignity The Power Grid


	sui-grid.middle.aligned.content(celled)
		sui-grid-row.center.aligned
			sui-grid-column(:width='3')
				img(src="alchemy-sulphuric.svg")


			sui-grid-column.middle.aligned(:width='13')
				docs-wireframe(name='centered-paragraph')
				img(src="ponteavmarinho.jpg" style="filter: brightness(70%) grayscale(85%)")
				h1.overlay-title.with.dignity(style="top: 35%") San Pavlov City
				h2.overlay-subtitle.with.dignity(style="top: 50%") Town Without Pity

		sui-grid-row
			sui-grid-column(:width='3')
				img(src="alchemy-sulphuric.svg")

			sui-grid-column(:width='10')
				img(src="biohazard.svg")
				img(src="biohazard.svg")
				img(src="biohazard.svg")

			sui-grid-column(:width='3')
				img(src="alchemy-sulphuric.svg")


</template>

<script>
export default {
	data() {
		return { open: false };
	},
	methods: {
		toggle() {
			this.open = !this.open;
		},
	},
};
</script>


<style lang="scss">
.container {
	text-align: center;
	min-height: 100vh;
	padding: 40px;
}

.material-icons, .fa, .fas, .far, .fab {
	vertical-align: middle;
}
.dignity {
	font-family: 'News Cycle', sans-serif !important;
	font-weight: 300 !important;
}

.container {
	position: relative;
	text-align: center;
	color: white;
}

.overlay-title {
	position: absolute;
	top: 50%;
	left: 50%;
	transform: translate(-50%, -50% )
}

overlay-subtitle {
	position: absolute;
	top: 75%;
	left: 50%;
	transform: translate(-50%, -50% )
}
</style>
