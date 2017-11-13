<template>
	<div class="app-header">
		<button class="menu-btn" v-on:click="headerMenuActive = true">
			<svg fill="#fff" height="24" viewBox="0 0 24 24" width="24" xmlns="http://www.w3.org/2000/svg">
			    <path d="M0 0h24v24H0z" fill="none"/>
			    <path d="M3 18h18v-2H3v2zm0-5h18v-2H3v2zm0-7v2h18V6H3z"/>
			</svg>
		</button>
		<div class="header-menu" v-bind:class="{ active: headerMenuActive }">
			<div class="header-menu-title">
				<button class="close-icon" v-on:click="headerMenuActive = false">
					<svg fill="#000000" height="24" viewBox="0 0 24 24" width="24" xmlns="http://www.w3.org/2000/svg">
					    <path d="M19 6.41L17.59 5 12 10.59 6.41 5 5 6.41 10.59 12 5 17.59 6.41 19 12 13.41 17.59 19 19 17.59 13.41 12z"/>
					    <path d="M0 0h24v24H0z" fill="none"/>
					</svg>
				</button>
			</div>
			<ul>
				<li v-on:click="headerMenuActive = false">
					<a href="#">
						<span class="icon">
							<svg fill="#999" height="24" viewBox="0 0 24 24" width="24" xmlns="http://www.w3.org/2000/svg">
							    <path d="M0 0h24v24H0z" fill="none"/>
							    <path d="M19.43 12.98c.04-.32.07-.64.07-.98s-.03-.66-.07-.98l2.11-1.65c.19-.15.24-.42.12-.64l-2-3.46c-.12-.22-.39-.3-.61-.22l-2.49 1c-.52-.4-1.08-.73-1.69-.98l-.38-2.65C14.46 2.18 14.25 2 14 2h-4c-.25 0-.46.18-.49.42l-.38 2.65c-.61.25-1.17.59-1.69.98l-2.49-1c-.23-.09-.49 0-.61.22l-2 3.46c-.13.22-.07.49.12.64l2.11 1.65c-.04.32-.07.65-.07.98s.03.66.07.98l-2.11 1.65c-.19.15-.24.42-.12.64l2 3.46c.12.22.39.3.61.22l2.49-1c.52.4 1.08.73 1.69.98l.38 2.65c.03.24.24.42.49.42h4c.25 0 .46-.18.49-.42l.38-2.65c.61-.25 1.17-.59 1.69-.98l2.49 1c.23.09.49 0 .61-.22l2-3.46c.12-.22.07-.49-.12-.64l-2.11-1.65zM12 15.5c-1.93 0-3.5-1.57-3.5-3.5s1.57-3.5 3.5-3.5 3.5 1.57 3.5 3.5-1.57 3.5-3.5 3.5z"/>
							</svg>
						</span>
						<span class="title">Настройки</span>
					</a>
				</li>
				<li v-on:click="headerMenuActive = false">
					<a href="#">
						<span class="icon">
							<svg fill="#999" height="24" viewBox="0 0 24 24" width="24" xmlns="http://www.w3.org/2000/svg">
							    <path d="M0 0h24v24H0z" fill="none"/>
							    <path d="M19.43 12.98c.04-.32.07-.64.07-.98s-.03-.66-.07-.98l2.11-1.65c.19-.15.24-.42.12-.64l-2-3.46c-.12-.22-.39-.3-.61-.22l-2.49 1c-.52-.4-1.08-.73-1.69-.98l-.38-2.65C14.46 2.18 14.25 2 14 2h-4c-.25 0-.46.18-.49.42l-.38 2.65c-.61.25-1.17.59-1.69.98l-2.49-1c-.23-.09-.49 0-.61.22l-2 3.46c-.13.22-.07.49.12.64l2.11 1.65c-.04.32-.07.65-.07.98s.03.66.07.98l-2.11 1.65c-.19.15-.24.42-.12.64l2 3.46c.12.22.39.3.61.22l2.49-1c.52.4 1.08.73 1.69.98l.38 2.65c.03.24.24.42.49.42h4c.25 0 .46-.18.49-.42l.38-2.65c.61-.25 1.17-.59 1.69-.98l2.49 1c.23.09.49 0 .61-.22l2-3.46c.12-.22.07-.49-.12-.64l-2.11-1.65zM12 15.5c-1.93 0-3.5-1.57-3.5-3.5s1.57-3.5 3.5-3.5 3.5 1.57 3.5 3.5-1.57 3.5-3.5 3.5z"/>
							</svg>
						</span>
						<span class="title">Настройки</span>
					</a>
				</li>
				<li v-on:click="headerMenuActive = false">
					<a href="#">
						<span class="icon">
							<svg fill="#999" height="24" viewBox="0 0 24 24" width="24" xmlns="http://www.w3.org/2000/svg">
							    <path d="M0 0h24v24H0z" fill="none"/>
							    <path d="M19.43 12.98c.04-.32.07-.64.07-.98s-.03-.66-.07-.98l2.11-1.65c.19-.15.24-.42.12-.64l-2-3.46c-.12-.22-.39-.3-.61-.22l-2.49 1c-.52-.4-1.08-.73-1.69-.98l-.38-2.65C14.46 2.18 14.25 2 14 2h-4c-.25 0-.46.18-.49.42l-.38 2.65c-.61.25-1.17.59-1.69.98l-2.49-1c-.23-.09-.49 0-.61.22l-2 3.46c-.13.22-.07.49.12.64l2.11 1.65c-.04.32-.07.65-.07.98s.03.66.07.98l-2.11 1.65c-.19.15-.24.42-.12.64l2 3.46c.12.22.39.3.61.22l2.49-1c.52.4 1.08.73 1.69.98l.38 2.65c.03.24.24.42.49.42h4c.25 0 .46-.18.49-.42l.38-2.65c.61-.25 1.17-.59 1.69-.98l2.49 1c.23.09.49 0 .61-.22l2-3.46c.12-.22.07-.49-.12-.64l-2.11-1.65zM12 15.5c-1.93 0-3.5-1.57-3.5-3.5s1.57-3.5 3.5-3.5 3.5 1.57 3.5 3.5-1.57 3.5-3.5 3.5z"/>
							</svg>
						</span>
						<span class="title">Настройки</span>
					</a>
				</li>
			</ul>
		</div>
	</div>
</template>

<script>
export default {
  name: 'appHeader',
  data () {
    return {
      msg: 'appHeader',
      headerMenuActive: false
    }
  }
}
</script>

<style lang="scss" scoped>

.app-header {
	display: -webkit-flex;
	display: -moz-flex;
	display: -ms-flex;
	display: -o-flex;
	display: flex;
	width: 100%;
	height: 40px;
	// background-color: #3d8aca;
	background-color: #0288D1;
}

.menu-btn {
	width: 40px;
	background: none;
	border: none;
	outline: none;
	cursor: pointer;

	&:hover {
		background-color: #3d8aca + 20;
	}
}

.header-menu {
	position: absolute;
	top: 0;
	left: -320px;
	width: 100%;
	max-width: 280px;
	height: 100%;
	background-color: #fff;
	box-shadow: 5px 0 5px rgba(0,0,0,0.1);
	transition: left 0.3s;

	&.active {
		left: 0;
	}

	.header-menu-title {
		display: flex;
		justify-content: flex-end;
		height: 40px;
		border-bottom: 1px solid #ECEFF1;

		.close-icon {
			display: flex;
			justify-content: center;
			align-items: center;
			width: 40px;
			height: 40px;
			border: none;
			background: none;
			outline: none;
			transition: background 0.3s;
			cursor: pointer;

			&:hover {
				// background: #ECEFF1;

				svg {
					transform: rotate(180deg);
					fill: #FF3D00;
				}
			}

			svg {
				display: block;
				fill: #607D8B;
				height: 22px;
				width: 22px;
				transition: transform 0.3s;
			}
		}
	}

	ul {
		list-style: none;

		li {
			border-bottom: 1px solid #ECEFF1;

			a {
				display: flex;
				align-items: center;
				padding: 0 10px;
				height: 40px;
				font: 400 13px/13px 'Roboto', sans-serif;
				color: #263238;
				text-decoration: none;

				&:hover {
					background-color: #ECEFF1;
				}

				.icon {
					margin-right: 8px;

					svg {
						display: block;
						fill: #607D8B;
						height: 22px;
						width: 22px;
					}
				}
			}
		}
	}
}

</style>