<script>
    // @ts-nocheck
    
        import Button from "./ui/button/button.svelte";
        import Resume from "$lib/icons/resume.svelte";
        import Tele from "$lib/icons/tele.svelte";
        import Info from "$lib/icons/info.svelte";
        import Github from "$lib/icons/github.svelte";
        import Flower from "$lib/icons/flower.svelte";
        import { page } from "$app/stores";
        import ThemeSwitch from "./themeSwitch.svelte";
    
    
       
    
    </script>
    
    <nav
        class="flex justify-between h-fit bg-secondary text-secondary-foreground py-1 px-4"
    >
        <div class="flex items-center text-xl">
    
            <div>
                <Flower/>
            </div>
            <Button
            class="{$page.url.pathname == '/' &&
                    'text-accent'}" 
            href="/" 
            variant="link">
             
                Shaima Fuad
    
            </Button>
            <ThemeSwitch/>
        </div>
    
    
        
       <div class="flex ">
        <div class="flex">
    
           
    
            <Button 
            class=" hidden sm:flex {$page.url.pathname == '/CV.pdf' &&
                    'text-accent'}"
            href="/CV.pdf" 
            variant="link">
                Resume
            </Button> <!--السيرة بالخط -->
    
            <Button 
            class=" text-xl {$page.url.pathname == '/CV.pdf' &&
                    'text-accent'} flex sm:hidden" 
            href="/CV.pdf" 
            variant="link">
                <Resume/>
            </Button> <!--السيرة بالرمز -->
    
            <Button 
            class=" hidden sm:flex {$page.url.pathname == '/about' &&
                    'text-accent'}" 
            href="/about" 
            variant="link">
                About
            </Button> <!--المعلومات بالخط -->
    
            <Button 
            class=" text-xl {$page.url.pathname == '/about' &&
                    'text-accent'} flex sm:hidden" 
            href="/about" 
            variant="link">
                <Info/>
            </Button> <!--المعلومات بالرمز -->
        </div>
        
    
    
        
            <div
             class="text-primary text-2xl text-primary/40 font-thin"> 
             
             <!--هذا الخط اللي بين الرسومات والكلمات-->
             |
            </div>
    
            <div>
                <Button 
            class="text-xl {$page.url.pathname == '/https://github.com/uiioj' &&
                    'text-accent'}" 
            href="https://github.com/uiioj" 
            variant="link">
                <Github />
            </Button>
    
            <Button 
            class="text-lg {$page.url.pathname == '/https://web.telegram.org/k/#@qur7illl' &&
                    'text-accent'}" 
            href="https://web.telegram.org/k/#@qur7illl" 
            variant="link">
                <Tele />
            </Button>
            </div>
    
       </div>
        
    </nav>
    
    
    
    