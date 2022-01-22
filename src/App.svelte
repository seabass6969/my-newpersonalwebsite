<script lang="ts">
    // all the component goes to here
    import test from './pages/blogcontain/test.svelte';

    import linux20220118 from './pages/blogcontain/linux20220118.svelte';
    import notfound from './pages/notfound.svelte';


    import blogs from './pages/blogs.svelte';
    import about from './pages/about.svelte';
    import home from './pages/home.svelte';
    import Topbar from './component/topbar.svelte';
    import Router from 'svelte-spa-router'
    var routes = {
        // general
        "/": home,
        "/about": about,
        "/blogs": blogs,
        // blog post link
        "/b/test": test,
        "/b/linux20220118" : linux20220118,
        // not found that use for error
        "/*": notfound,
    }
    // <Topbar/>
    // <Markdown markdown={test}/>
</script>

<main>
    <Topbar/> 
    <Router {routes}/>
</main>

