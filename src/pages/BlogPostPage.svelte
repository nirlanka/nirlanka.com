<script>
    export let postId;

    let article;

    (async () => {
        const articleRes = await fetch(`https://dev.to/api/articles/${postId}`);
        article = await articleRes.json();
    })();
</script>

{#if !article}
    <div>Loading article...</div>
{/if}

{#if article}
    <div>
        <h2>{article.title}</h2>
        <p>{article.description}</p>
    </div>
{/if}