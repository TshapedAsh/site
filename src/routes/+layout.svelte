<script lang="ts">
  import '../app.css';
  import { browser } from '$app/environment';
  import { theme } from '$lib/stores/theme';
  import ThemeToggle from '$lib/ThemeToggle.svelte';
  $: if (browser) {
    document.documentElement.className = $theme;
  }
</script>
<ThemeToggle class="fixed top-4 right-4" />
<slot />
