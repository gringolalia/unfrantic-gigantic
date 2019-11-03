<template lang="pug">
	div
		.ui.large.fixed.top.secondary.menu.with.dignity(style="background-color: white;")
			a.active.item
				i.large.settings.icon
				|  Engenho Novo LLC
			.ui.computer.only.grid
				a.item(href="/abelard")
					| In Media Res
				a.item(href="/augustine")
					| Anagnorisis
				a.item(href="/aristotle")
					| Hamartia

			.ui.simple.dropdown.item
				| Rhetors
				i.dropdown.icon

				.left.menu
					a.item(href="/aristotle")
						i.large.chess.rook.icon
						| Aristotle

					a.item(href="/cicero")
						i.material-icons flight
						| Cicero

					a.item(href="/sophists")
						i.material-icons beach_access
						| Sophists

					a.item(href="/quintillian")
						i.material-icons alternate_email
						| Quintillian

					a.item(href="/isocrates")
						i.material-icons zoom_in
						| Isocrates

					a.item(href="/abelard")
						i.material-icons translate
						| Abelard
					a.item(href="/toulmin")
						i.material-icons flare
						| Stephen Toulmin
					a.item(href="/burke")
						i.material-icons flash_auto
						| Kenneth Burke
					a.item(href="/augustine")
						i.large.chess.board.icon
						| Augustine
					a.item(href="/boethius")
						i.material-icons waves
						| Boethius

			.right.menu
				.ui.computer.only.grid
					a.ui.item(href='/' style="margin-right: 20px")
						i.fa.fa-tv
						|  Mimesis
		nuxt

		script.
			$('.ui.dropdown').dropdown();
</template>

<style>
@import url(https://cdn.jsdelivr.net/npm/semantic-ui@2.4.0/dist/semantic.min.css);
@import url(https://stackpath.bootstrapcdn.com/font-awesome/4.7.0/css/font-awesome.min.css);
@import url(https://use.fontawesome.com/releases/v5.5.0/css/all.css);
@import url(https://fonts.googleapis.com/css?family=News+Cycle|Material+Icons);

html {
	font-family: "News Cycle", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
	font-size: 16px;
	word-spacing: 1px;
	-ms-text-size-adjust: 100%;
	-webkit-text-size-adjust: 100%;
	-moz-osx-font-smoothing: grayscale;
	-webkit-font-smoothing: antialiased;
	box-sizing: border-box;
}

*, *:before, *:after {
	box-sizing: border-box;
	margin: 0;
}

/* Rules for sizing the icon. */
.material-icons.md-18 { font-size: 18px; }
.material-icons.md-24 { font-size: 24px; }
.material-icons.md-36 { font-size: 36px; }
.material-icons.md-48 { font-size: 48px; }
.material-icons.md-64 { font-size: 64px; }

/* Rules for using icons as black on a light background. */
.material-icons.md-dark { color: rgba(0, 0, 0, 0.54); }
.material-icons.md-dark.md-inactive { color: rgba(0, 0, 0, 0.26); }

/* Rules for using icons as white on a dark background. */
.material-icons.md-light { color: rgba(255, 255, 255, 1); }
.material-icons.md-light.md-inactive { color: rgba(255, 255, 255, 0.3); }

i, .icon, .material-icons, .fa {
	margin-right: 10px;
}

.left {
	text-align: left;
}
.right {
	text-align: right;
}
.center {
	text-align: center;
}

img {
	margin-top: 25px;
	margin-bottom: 25px;
}
</style>
