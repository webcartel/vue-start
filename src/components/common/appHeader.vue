<template>
	<div class="app-header">
		<button class="menu-btn">
			<svg fill="#fff" height="24" viewBox="0 0 24 24" width="24" xmlns="http://www.w3.org/2000/svg">
			    <path d="M0 0h24v24H0z" fill="none"/>
			    <path d="M3 18h18v-2H3v2zm0-5h18v-2H3v2zm0-7v2h18V6H3z"/>
			</svg>
		</button>
	</div>
</template>

<script>
export default {
  name: 'appHeader',
  data () {
    return {
      msg: 'appHeader'
    }
  }
}
</script>

<style scoped>

.app-header {
	display: -webkit-flex;
	display: -moz-flex;
	display: -ms-flex;
	display: -o-flex;
	display: flex;
	width: 100%;
	height: 40px;
	background-color: #3d8aca;
}

.menu-btn {
	width: 40px;
	background: none;
	border: none;
	outline: none;
}

</style>