<script lang="ts">
  import Button from "@/components/ui/button/button.svelte";
  import { Calendar } from "$lib/components/ui/calendar";
  import { today, getLocalTimeZone } from "@internationalized/date";
 
  let value = today(getLocalTimeZone());
</script>

<h1>Welcome to SvelteKit</h1>
<p>
  Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation
</p>
<Button>Click me</Button>
<Calendar bind:value class="rounded-md border" />
