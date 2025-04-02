<script lang="ts">

    import SignaturePad from 'signature_pad';
    import { onMount, getContext } from 'svelte';

    let canvas: HTMLCanvasElement;
    let pad: SignaturePad;


    onMount(() => {
        pad = new SignaturePad(canvas, {
                penColor: 'black',
            });

    })

</script>


<h1>Welcome to SvelteKit</h1>
<p>Visit <a href="https://svelte.dev/docs/kit">svelte.dev/docs/kit</a> to read the documentation</p>


<canvas
    style="width: 40rem; height: 20rem; border: 1px solid black"
    bind:this={canvas}
    class="rounded border">
</canvas>
