<script>
    import "../app.css";
    import { ModeWatcher } from "mode-watcher";
    import Navbar from "$lib/components/Navbar.svelte";
</script>
<!-- svelte-ignore missing-declaration -->
<Navbar/>
<ModeWatcher/>
<slot></slot>