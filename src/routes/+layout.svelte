<script>
    import "../app.css";
    import { ModeWatcher } from "mode-watcher";
    import Navbar from "$lib/components/Navbar.svelte";
    import Footer from "$lib/components/Footer.svelte";


</script>
<!--هنا الاشياء اللي تكون موجودة بكل النوافذ-->

<Navbar/>

<ModeWatcher />

<main class="min-h-[calc(100vh-7rem)]">
    <slot></slot>
</main>

<Footer></Footer>
