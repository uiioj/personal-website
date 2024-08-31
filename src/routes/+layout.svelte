<script>
    import "../app.css";
    import { ModeWatcher } from "mode-watcher";
    import Navbar from "$lib/components/Navbar.svelte";
    import Footer from "$lib/components/Footer.svelte";


</script>
<!--هنا الاشياء اللي تكون موجودة بكل النوافذ-->

<Navbar/>

<ModeWatcher />

<slot></slot>

<Footer></Footer>
