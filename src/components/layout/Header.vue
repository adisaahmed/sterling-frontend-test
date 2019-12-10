<template>
	<div>
		<b-navbar toggleable="lg" type="dark" variant="info">
			<b-navbar-brand href="#">
				STERLING
			</b-navbar-brand>

			<b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

			<b-collapse id="nav-collapse" is-nav>
				<!-- Right aligned nav items -->
				<b-navbar-nav class="ml-auto">
					<b-nav-form>
						<b-form-input size="sm" class="mr-sm-2" placeholder="Search"></b-form-input>
						<b-button size="sm" class="my-2 my-sm-0" type="submit">Search</b-button>
					</b-nav-form>

					<b-nav right>
						<b-nav-item active>
							<router-link to="/">
								Home
							</router-link>
						</b-nav-item>
						<b-nav-item>
							<router-link to="/about">
								People
							</router-link>
						</b-nav-item>
						<b-nav-item>Planets</b-nav-item>
						<b-nav-item>Starships</b-nav-item>
					</b-nav>
				</b-navbar-nav>
			</b-collapse>
		</b-navbar>
	</div>
</template>

<script>
	export default {
		name: "Header"
	}
</script>