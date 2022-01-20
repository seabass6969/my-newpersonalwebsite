<style>
</style>
<script>
  import MarkdownIt from 'markdown-it'
  export let markdown = ''

  const md = new MarkdownIt()

  const rendered = md.render(markdown)
</script>

<div>
  {@html rendered}
</div>

