<script lang="ts">
    import type {Day} from '$lib/types';
    import Talks from "./Talks.svelte";
    import Speakers from "./Speakers.svelte";
    export let days: Day[];
</script>

<ul>
    {#each days as day}
    <div>
        <Talks talks={day.talks} />
        <Speakers speakers={day.speakers} />
    </div>
    {/each}
</ul>