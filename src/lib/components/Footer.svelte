<script>
        import Button from "./ui/button/button.svelte";
        import { page } from "$app/stores";
        import Github from "$lib/icons/github.svelte";
        import Tele from "$lib/icons/tele.svelte";
        import number from "$lib/icons/number.svelte";
    import Number from "$lib/icons/number.svelte";



</script>


<footer class="bg-background text-foreground py-5 px-5">
    <div class="max-w-screen-2xl flex justify-between items-center mx-auto text-primary-foreground">


<span><!--اللي عاليسار -->
    <div>👩🏻‍💻 + 👩🏻‍🎨 by me</div>
<div>© {(new Date()).getFullYear()}</div>
</span>



<span class="flex items-center"><!--اللي عاليمين-->
    <Button 
        class="text-2xl   {$page.url.pathname == '/https://github.com/uiioj' &&
                'text-accent'}" 
        href="https://github.com/uiioj" 
        variant="link">
            <Github />
        </Button>

        <div
         class="text-primary text-2xl text-primary/40 font-thin"> 
         
         <!--هذا الخط اللي بين الرسومات والكلمات-->
         |
        </div>

        <Button 
        class="text-xl  {$page.url.pathname == '/https://web.telegram.org/k/#@qur7illl' &&
                'text-accent'}" 
        href="https://web.telegram.org/k/#@qur7illl" 
        variant="link">
            <Tele />
        </Button>


        <div
         class="text-primary text-2xl text-primary/40 font-thin"> 
         <!--الفاصل-->
         |
        </div>

        <Button 
        class="text-lg {$page.url.pathname == '/tel:0556540378' &&
                'text-accent'}" 
        href="tel:0556540378" 
        variant="link">
           <Number/>
        </Button>
    </span>



    </div>
</footer>