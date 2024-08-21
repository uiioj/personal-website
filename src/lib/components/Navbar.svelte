<script>
// @ts-nocheck

    import Button from "./ui/button/button.svelte";
    import Resume from "$lib/icons/resume.svelte";
    import Tele from "$lib/icons/tele.svelte";
    import Info from "$lib/icons/info.svelte";
    import Github from "$lib/icons/github.svelte";
    import { page } from "$app/stores";


    const links = [
        {
            text: 'Resume',
            href: '/resume'
        },
        {
            text:'About',
            href: '/about'
        }
    ]

</script>

<nav
    class="flex justify-between w-[100dvw] h-fit bg-secondary text-secondary-foreground py-1 px-4"
>
    <div class="flex items-center gap-2 text-xl">
        <div class="bg-primary w-5 h-5 ms-3" />
        <Button variant="link">
            Shaima Fuad

        </Button>
    </div>

    <div class="flex items-center p-1 ">
    <div class="hidden sm:flex">
        {#each links as link}
        <Button
        class="{$page.url.pathname == link.href &&
                  link.text}"
                  href={link.href}
                  variant="link"
                  >{link.text}
  
        </Button>
  
       {/each}
    </div>

    

        <div
         class="text-primary text-2xl text-primary/40 font-thin">
         |
        </div>

        <Button 
        class="text-2xl {$page.url.pathname == '/https://github.com/uiioj' &&
                'text-accent'}" 
        href="/" 
        variant="link">
            <Github />
        </Button>

        <Button 
        class="text-xl {$page.url.pathname == '/https://web.telegram.org/k/#@qur7illl' &&
                'text-accent'}" 
        href="/" 
        variant="link">
            <Tele />
        </Button>

        
    </div>


</nav>
