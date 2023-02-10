<script lang="ts">
    import type {Speaker} from '$lib/types';
    export let speakers: Speaker[];
</script>

<div class="bg-blue-400">
    <ul>
        {#each speakers as speaker}
        <h4 class="text-lg mt-10">Speaker</h4>
        <li>{speaker.name}</li>
        <li><img src="{speaker.imageUrl}" alt="Bild"></li> 
        {/each}
    </ul>
</div>