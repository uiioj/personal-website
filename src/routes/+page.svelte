<script>
	// @ts-nocheck

	import Button from "$lib/components/ui/button/button.svelte";
	import { page } from "$app/stores";
	import UQU from "$lib/icons/UQU.svelte";
	import Computer from "$lib/icons/computer.svelte";
	import Container from "$lib/components/Container.svelte";
	import Arrow from "$lib/icons/arrow.svelte";
    import ProjectCard from "$lib/components/ProjectCard.svelte";


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


<div> <!--الحاوية حق كل شي-->


	<div
		class=" text-secondary-foreground font-semibold p-10 px-10 flex items-center justify-between flex-col sm:flex-row animate-text ">
		<!--الفقرة الاولى-->

		<div>
			<div class="text-3xl font-bold my-8">
				HELLO!
			</div>

			<div class="flex items-center text-nowrap flex-wrap gap-1.5">
				I'm Shaima - a
				<Button
					class="text-md {$page.url.pathname == '/https://www.mtu.edu/cs/what/' && 'text-accent'} px-0 w-fit hover:text-[#f16349] "
					style="text-decoration:underline;text-decoration-color:tomato;"
					href="https://www.mtu.edu/cs/what/"
					variant="link">
					Computer Science
				</Button>
				<Computer/>


				Student at
				<Button
					class=" text-md {$page.url.pathname == 'https://uqu.edu.sa/' &&
               'text-accent'} px-0 w-fit hover:text-[#f16349] "
					style="text-decoration: underline;text-decoration-color:tomato;"
					href="https://uqu.edu.sa/"
					variant="link">
					Um Al-Qura <div class="m-1">
						<UQU/>
					</div>

				</Button>
				University

			</div>

			I graduated 🎓 from
			<Button
				class=" text-md {$page.url.pathname == '/https://x.com/moe_mhc_25_3003?lang=ar' &&
          'text-accent'} px-0 w-fit hover:text-[#f16349] "
				style="text-decoration: underline;text-decoration-color:tomato;"
				href="https://x.com/moe_mhc_25_3003?lang=ar"
				variant="link">
				Second high school
			</Button>
			with a GPA of 99.78%
		</div>

		<div class="flex items-end justify-end">
			<!-- svelte-ignore a11y-img-redundant-alt -->
			<img class="h-auto w-auto min-w-96 mt-16" src="/image3.webp" alt="image"/>

		</div>

	</div><!--خلصنا الاولى -->


	<div class=""> <!--الثانيه-->
		<div class="text-secondary-foreground font-bold text-3xl px-10 animate-text flex gap-2 animate-text ">
			CHECK OUT MY PROJECTS
			<Arrow/>
		</div>

    
		<div class=" md:flex justify-center items-center">
			<Container >
				<div class=" rounded-full flex items-center justify-center shadow-xl h-[20rem] w-[20rem] bg-secondary ">
	
					<!-- svelte-ignore a11y-missing-attribute -->
					 
					<img src="/calculator.png" class=" h-[20rem] w-[20rem] "/>
				</div>
				<div>
				<ProjectCard >
					<div class="text-2xl font-semibold text-secondary-foreground">
						Calculator</div> 
	
					<div >
						<div class="m-4 text-lg text-secondary-foreground">
						<div>▪️ Easy to use</div>
						<div>▪️ Fast and helpful</div>
						<div>▪️ Accuracy in results </div>
						<div>▪️ Attention in details</div>
	
						</div>
					
						
					
					<Button
						class=" text-md {$page.url.pathname == '/https://bright-manatee-72e92c.netlify.app/' &&
				   'text-accent'} px-0 w-16 rounded-2xl"
						
						href="https://bright-manatee-72e92c.netlify.app/">
						try it!
						
					
	
					</Button>
					
				</ProjectCard>
			</div>
		
		</Container>
	
	
	
	
	
			<Container >
				<div class=" rounded-full flex justify-center items-center shadow-xl h-[20rem] w-[20rem] bg-secondary mx-auto ">
	
					<!-- svelte-ignore a11y-missing-attribute -->
					<img src="/todolist.png" class="h-[20rem] w-[20rem]"/>
				</div>
				<ProjectCard >
	
					<div class="text-2xl font-semibold text-secondary-foreground">
						To-Do-List</div> 
	
					<div >
						<div class="m-4 text-lg text-secondary-foreground">
	
						<div>▪️ Time management</div>
						<div>▪️ Security and privacy</div>
						<div>▪️ Accurate time setting</div>
						<div>▪️ Consistency and arrangement</div>
	
						</div>
					
						
					
					<Button
						class=" text-md {$page.url.pathname == '/https://todolistshaima.netlify.app/' &&
				   'text-accent'} px-0 w-16 rounded-2xl"
						
						href="https://todolistshaima.netlify.app/">
						try it!
						
					
	
					</Button>
					
	
	
				</ProjectCard>
			</Container>
	
		</div>


	   

	</div>
</div>






