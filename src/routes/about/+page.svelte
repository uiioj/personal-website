<script lang="ts">
    import Button from "$lib/components/ui/button/button.svelte";
    import AboutCard from "$lib/components/AboutCard.svelte"
    import { page } from "$app/stores";
    

</script>

<div class="max-w-screen-md px-4 mx-auto pt-16 py-16 text-secondary-foreground flex flex-col gap-7 "><!--حقهم كلهم -->


    <h1 class=" mx-auto w-fit text-4xl font-bold">
        NICE TO MEET YOU!
    </h1>

    <AboutCard >
        I'm a Computer Science student with a passion for the world of technology and programming. One of the things that sets me apart is my love for reading and staying informed 📚. 
        I enjoy discovering and learning new things because knowledge is power! Alongside my studies, I have a keen interest in hobbies; whether it's sports, video games, or even learning new skills. I see hobbies not just as entertainment but as a way to develop oneself and find a balance between personal life and academics 💡. Who said university life has to be serious 24/7? There should always be time for fun and exploration!

        Good luck! 🚀
   </AboutCard>

   <AboutCard >
    <div class="flex flex-col md:flex-row">
        <!--البوكس حق الكتب-->

        <div class="text-xl font-semibold">
         My through lists
        
        </div>


        <!--<Button 
            class=" text-xl {$page.url.pathname == '/' &&
                    'text-accent'} flex sm:hidden" 
            href="/" 
            variant="link">
                
            </Button> -->

        <div> 
           <Button class="{$page.url.pathname == '/' &&
                    'text-accent'} "
                    href="/"
                    variant="link"
                    style="text-decoration: underline;text-decoration-color:tomato;">
                    سابغات

           </Button>
        
         </div>



         <div>
            اللي لسا ماخلصتها
         </div>


    </div>
   </AboutCard>

   <AboutCard>
    ميمز او عبارة تعجبني
   </AboutCard>

    

</div>