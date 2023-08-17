<script lang="ts">
	import { Canvas } from '@threlte/core';
	import Scene from './Scene.svelte';
	import { SheetObject, Studio, Theatre } from '@threlte/theatre';
</script>

<Studio enabled={true} />
<Canvas
	colorManagementEnabled
	rendererParameters={{
		precision: 'highp',
		antialias: true,
		logarithmicDepthBuffer: true,
		powerPreference: 'high-performance'
	}}
>
	<Theatre>
		<Scene />
	</Theatre>
</Canvas>
