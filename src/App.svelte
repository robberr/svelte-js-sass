
<!--//  type="text/ts"  lang="ts"  <script lang="typescript" >-->
<script >
 
  export let name;
  import face from './face.svelte';
  import input from './input.svelte';
  let say='hi';
  setTimeout(()=>{say='bye';},3000)
</script>
<input max="20" label="hello there"/>


<main>
	<h1>Good {name}!</h1>
	
</main>
<!--type="text/scss"  lang="scss"-->
<style type="text/scss">
  @import '../public/global.scss';
  @import './main.scss';

 
</style>

<!--<template lang="pug" type="text/pug">
  h1 Hello!
  br
  input(bind:value="{label}")
  br
  Nested("{label}")
</template>-->

<h2>Hello! how is this {name}!</h2>
<div class="flecole0">
  <slot>flecole0</slot>
  <h3>exellent {name}!</h3>
</div>
<div class="flecoau0">
  <slot>flecoau0</slot>
  <h3>satisfy {name}!</h3>
</div>
<div class="flecori50">
  <slot>flecori50</slot>
  <h3>faz {name}!</h3>
</div>
<div class="fleroau">
  <slot>fleroau</slot>
  <face size="4"/>
  <face size="10"/>
  <face />
  <p>yess SASS is working!</p>
</div>
<div class="flerole">
  <slot>flerole</slot>
  <p>yess SASS is working!</p>
</div>

<div class="flerori">
  <slot>flerori</slot>
  <h1>say:{say}</h1>
  <p>yess SASS is working!</p>
</div>

<footer class="footer">
  <p>

    Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn how to build Svelte apps.
  </p>
</footer>

