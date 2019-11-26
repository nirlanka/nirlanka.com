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
        <div>
            <h2>{article.title}</h2>
            <p>{article.description}</p>
        </div>
    </Link>
    {/each}
{/if}