<script>
	import { Router, Route } from "svelte-routing";

	import HomePage from './pages/HomePage.svelte';
</script>

<main>
  <Router>
    <Route path="">
      <HomePage />
    </Route>
  </Router>
</main>