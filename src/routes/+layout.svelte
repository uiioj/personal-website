<script>
    import "../app.css";
    import { ModeWatcher } from "mode-watcher";
    import Navbar from "$lib/components/Navbar.svelte";


</script>
<!--هنا الاشياء اللي تكون موجودة بكل النوافذ-->

<Navbar/>

<ModeWatcher />

<slot></slot>
