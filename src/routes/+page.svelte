<script setup lang="ts">
import {authClient} from "hulk-sdk";

const client = new authClient("main", "TetsApp");

async function login() {
	const address = await client.login();
	console.log(address);
}
</script>

<!-- YOU CAN DELETE EVERYTHING IN THIS PAGE -->
<div class="container h-full mx-auto flex justify-center items-center">
	<div class="space-y-10 text-center flex flex-col items-center">
		<h2 class="h2">Welcome to Skeleton.</h2>
		<button class="btn variant-filled" on:click={login}>Login</button>
	</div>
</div>
