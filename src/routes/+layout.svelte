<script>
import "../app.css";
import { ModeWatcher } from "mode-watcher";
import Navbar from "$lib/components/Navbar.svelte";
import Themeswitch from "$lib/components/Themeswitch.svelte";
</script>
<Navbar/>
<ModeWatcher/>
<slot></slot>


