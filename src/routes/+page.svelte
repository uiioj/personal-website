<script >
// @ts-nocheck

    import Button from "$lib/components/ui/button/button.svelte";
    import { page } from "$app/stores";
    import UQU from "$lib/icons/UQU.svelte";
    import Computer from "$lib/icons/computer.svelte";
    import Container from "$lib/components/Container.svelte";
    

</script>

<style>
    @keyframes slideUp {
      0% {
        opacity: 0;
        transform: translateY(100%);
      }
      100% {
        opacity: 1;
        transform: translateY(0);
      }
    }
  
    .animate-text {
      animation: slideUp 1s ease-out forwards;
    }
  </style>


<div class=" text-secondary-foreground font-semibold p-10 px-10 flex items-center justify-between flex-row animate-text "> <!--الفقرة الاولى-->

  <div>
    <div class="text-3xl font-bold my-8">
        HELLO!
    </div>

    <div class="flex items-center  gap-1.5">
        I'm Shaima - a 
        <Button
    class="text-md {$page.url.pathname == '/https://www.mtu.edu/cs/what/' && 'text-accent'} px-0 w-fit hover:text-[#f16349] " 
    style="text-decoration:underline;text-decoration-color:tomato;"        
    href="https://www.mtu.edu/cs/what/" 
    variant="link">
     Computer Science
</Button>
 <Computer/>



     Student at <Button
     class=" text-md {$page.url.pathname == 'https://uqu.edu.sa/' &&
             'text-accent'} px-0 w-fit hover:text-[#f16349] " 
     style ="text-decoration: underline;text-decoration-color:tomato;"        
     href="https://uqu.edu.sa/" 
     variant="link">
     Um Al-Qura

</Button> University 

    </div>

I graduated from <Button
class=" text-md {$page.url.pathname == '/https://x.com/moe_mhc_25_3003?lang=ar' &&
        'text-accent'} px-0 w-fit hover:text-[#f16349] " 
style ="text-decoration: underline;text-decoration-color:tomato;"          
href="https://x.com/moe_mhc_25_3003?lang=ar" 
variant="link">
Second high school</Button> with a GPA of 99.78% </div>

<div class="flex items-end  justify-end h-96 w-96">
    <img src="/image3.webp" alt="image"/>

</div>

</div>




<div>
    <div class="text-secondary-foreground font-bold text-3xl px-10 animate-text">
        CHECK OUT MY PROJECTS
    </div>
    <Container>

    </Container>

   

</div>






