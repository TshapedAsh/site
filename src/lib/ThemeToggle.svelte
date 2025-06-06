<script lang="ts">
  import { theme, toggleTheme } from '$lib/stores/theme';
</script>
<button on:click={toggleTheme} class="p-2 rounded bg-gray-200 dark:bg-gray-700">
  Toggle { $theme === 'light' ? 'Dark' : 'Light' }
</button>
