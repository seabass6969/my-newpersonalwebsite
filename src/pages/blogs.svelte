<style>
.title {
    color:lime;
    font-size: 4vw;
}
.description {
color: rosybrown;
}
.flags {
padding-left: 4px;
padding-right: 4px;
}
</style>

<script>
    const blogpage = [
        {title: "test", description: "it is a test page", url: "/#/b/test", flags: ["test", "testing"]},
        {title: "linux tips 1", description: "tips 1 for linux", url: "/#/b/linux20220118", flags: ["linux", "tips"]}];

</script>
<h1>list of all blog post I post 😉:</h1>
{#each blogpage as {title, description, url, flags}}
    <a class="title" href={url} >{title}</a>
    <br>
    {#each flags as flag}
        <div class="flags" style="display:inline">#{flag}</div>
    {/each}
    <br>
    <a class="description" href={url}>{description}</a>
    <br>
{/each}
