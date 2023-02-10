<script lang="ts">
    import type {Talk} from '$lib/types';
    export let talks: Talk[];
    console.log(talks)
</script>

<ul>
    {#each talks as talk}
    <li><span class="font-bold">Talk title:</span> {talk.title}</li>
    {/each}
</ul>