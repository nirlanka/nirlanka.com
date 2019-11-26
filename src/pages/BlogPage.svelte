<script>
    import { Link } from "svelte-routing"

    import site from '../data/site';

    let articles;

    (async () => {
        const jsonRes = await fetch(`https://dev.to/api/articles?username=${site.devtoUsername}`);
        articles = await jsonRes.json();
    })();

    $: console.log(articles);
</script>

{#if !articles}<div>Loading posts...</div>{/if}

{#if articles}
    {#each articles as article}
    <Link to={`/blog/${article.id}`}>
        <div>{article.title}</div>
        <div>{article.description}</div>
    </Link>
    {/each}
{/if}