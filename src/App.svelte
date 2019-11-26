<script>
	import { Router, Route } from "svelte-routing";

	import pageId from './data/pageId';
	import HomePage from './pages/HomePage.svelte';
	import BlogPage from './pages/BlogPage.svelte';
	import BlogPostPage from './pages/BlogPostPage.svelte';

	import Header from './components/Header.svelte';
</script>

<link rel="stylesheet" type="text/css" href="reset.css">
<link rel="stylesheet" type="text/css" href="simple-grid.css">
<link rel="stylesheet" type="text/css" href="home.css">

<main>
  <Router>
    <Route path="/">
      <Header currentPageId={pageId.home} />
      <HomePage />
    </Route>
	<Route path="/blog">
      <Header currentPageId={pageId.blog} />
      <BlogPage />
    </Route>
	<Route path="/blog/:id" let:params>
      <Header currentPageId={pageId.blog} />
      <BlogPostPage postId={params.id} />
    </Route>
  </Router>
</main>