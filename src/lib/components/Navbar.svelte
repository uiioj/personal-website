<script>
// @ts-nocheck

    import Button from "./ui/button/button.svelte";
    import Resume from "$lib/icons/resume.svelte";
    import Tele from "$lib/icons/tele.svelte";
    import Info from "$lib/icons/info.svelte";
    import Github from "$lib/icons/github.svelte";
    import Flower from "$lib/icons/flower.svelte";
    import { page } from "$app/stores";


   

</script>

<nav
    class="flex justify-between w-[100dvw] h-fit bg-secondary text-secondary-foreground py-1 px-4"
>
    <div class="flex items-center gap-2 text-xl">

        <div>
            <Flower/>
        </div>
        <Button
        class="{$page.url.pathname == '/shaima' &&
                'text-accent'} flex md:hidden" 
        href="/shaima" 
        variant="link">
         
            Shaima Fuad

        </Button>
    </div>

    
    <Button 
        class=" {$page.url.pathname == '/resume' &&
                'text-accent'}"
        href="/resume" 
        variant="link">
            Resume
        </Button> <!--السيرة بالخط -->

        <Button 
        class=" text-xl {$page.url.pathname == '/resume' &&
                'text-accent'} flex md:hidden" 
        href="/resume" 
        variant="link">
            <Resume/>
        </Button> <!--السيرة بالرمز -->

        <Button 
        class=" {$page.url.pathname == '/about' &&
                'text-accent'}" 
        href="/about" 
        variant="link">
            About
        </Button> <!--المعلومات بالخط -->

        <Button 
        class=" text-xl {$page.url.pathname == '/about' &&
                'text-accent'} flex md:hidden" 
        href="/about" 
        variant="link">
            <Info/>
        </Button> <!--المعلومات بالرمز -->
    


    
        <div
         class="text-primary text-2xl text-primary/40 font-thin"> 
         
         <!--هذا الخط اللي بين الرسومات والكلمات-->
         |
        </div>

        <Button 
        class="text-2xl {$page.url.pathname == '/https://github.com/uiioj' &&
                'text-accent'}" 
        href="/https://github.com/uiioj" 
        variant="link">
            <Github />
        </Button>

        <Button 
        class="text-xl {$page.url.pathname == '/https://web.telegram.org/k/#@qur7illl' &&
                'text-accent'}" 
        href="/https://web.telegram.org/k/#@qur7illl" 
        variant="link">
            <Tele />
        </Button>

    

        


</nav>
