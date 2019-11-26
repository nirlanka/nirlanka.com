<script>
    import { Link } from "svelte-routing"

    import pageId from '../data/pageId';
    import site from '../data/site';

    export let currentPageId = pageId.home;
</script>

<nav>
    <h1>{site.title}</h1>

    {#if currentPageId !== pageId.home}
        <Link to="/">Home</Link>
    {/if}
    {#if currentPageId !== pageId.blog}
        <Link to="/blog/">Blog</Link>
    {/if}
</nav>
