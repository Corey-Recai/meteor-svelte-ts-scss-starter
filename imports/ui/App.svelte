<script lang="ts">
    import { Router, Link, Route } from "svelte-routing";

    import Home from "./views/Home/Home.svelte";
    import Blog from "./views/Blog/Blog.svelte";

    export let url = "";
</script>

<Router {url}>
    <Route path="blog/:id" component={Blog} />
    <Route path="/" component={Home} />
</Router>
