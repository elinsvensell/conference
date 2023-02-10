<script lang="ts">
    import type {Conference} from '$lib/types';
    export let conference: Conference;
</script>

<div class="bg-green-400">
    <h1 class="text-xl">{conference.title}</h1>
    <h2>{conference.description}</h2>
    <h3>Where: {conference.location} - {conference.venue}</h3>
    <h3>When: {conference.startDate} - {conference.endDate}</h3>
</div>