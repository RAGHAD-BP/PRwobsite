<script>
    import "../app.css";
    import { ModeWatcher } from "mode-watcher";
    import Navbar from "$lib/components/Navbar.svelte";
    import Footer from "$lib/components/Footer.svelte";
</script>
<!-- svelte-ignore missing-declaration -->
<Navbar/>
<ModeWatcher/>
<slot/>
<Footer/>