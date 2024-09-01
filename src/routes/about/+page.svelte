<script lang="ts">
    import Button from "$lib/components/ui/button/button.svelte";
    import AboutCard from "$lib/components/AboutCard.svelte";
    import { page } from "$app/stores";
    import * as Dialog from "$lib/components/ui/dialog";
</script>

<div
    class="max-w-screen-md px-4 mx-auto pt-16 py-16 text-secondary-foreground flex flex-col gap-7"
>
    <!--حقهم كلهم -->

    <h1 class=" mx-auto w-fit text-4xl font-bold">NICE TO MEET YOU!</h1>
    <div class="text-justify">
        <AboutCard>
            I'm a Computer Science student with a passion for the world of
            technology and programming. One of the things that sets me apart is
            my love for reading and staying informed 📚. I enjoy discovering and
            learning new things because knowledge is power! Alongside my
            studies, I have a keen interest in hobbies; whether it's sports,
            video games, or even learning new skills. I see hobbies not just as
            entertainment but as a way to develop oneself and find a balance
            between personal life and academics 💡. Who said university life has
            to be serious 24/7? There should always be time for fun and
            exploration! 
            <div>
                Good luck! 🚀
            </div>
        </AboutCard>
    </div>
    <div>
        <AboutCard>
            <div class="text-xl font-semibold text-center p-4">My through lists :</div>

            <!--البوكس حق الكتب-->
            <div class="flex justify-center items-center text-center">
                <div>
                    <!--البوكس الاول-->

                    <div>
                        <Button
                            class="{$page.url.pathname == '/' &&
                                'text-accent'} "
                            href="/"
                            variant="link"
                            style="text-decoration: underline;text-decoration-color:tomato;"
                        >
                            سابغات
                        </Button>

                        <script lang="ts">
                            import * as Dialog from "$lib/components/ui/dialog";
                           </script>
                            
                           <Dialog.Root>
                            <Dialog.Trigger class="font-semibold"
                            style="text-decoration: underline;text-decoration-color:tomato;">سابغات</Dialog.Trigger>
                            <Dialog.Content>
                             <Dialog.Header>
                              <Dialog.Title >  كتاب سابغات 📙</Dialog.Title>
                              <Dialog.Description>
                               This action cannot be undone. This will permanently delete your account
                               and remove your data from our servers.
                              </Dialog.Description>
                             </Dialog.Header>
                            </Dialog.Content>
                           </Dialog.Root>
                    </div>

                    <div>
                        <Button
                            class="{$page.url.pathname == '/' &&
                                'text-accent'} "
                            href="/"
                            variant="link"
                            style="text-decoration: underline;text-decoration-color:tomato;"
                        >
                            فاتتني صلاة
                        </Button>
                    </div>

                    <div>
                        <Button
                            class="{$page.url.pathname == '/' &&
                                'text-accent'} "
                            href="/"
                            variant="link"
                            style="text-decoration: underline;text-decoration-color:tomato;"
                        >
                            الحفرة السعيدة
                        </Button>
                    </div>
                    <div>
                        <Button
                            class="{$page.url.pathname == '/' &&
                                'text-accent'} "
                            href="/"
                            variant="link"
                            style="text-decoration: underline;text-decoration-color:tomato;"
                        >
                            فقه الأسماء الحسنى
                        </Button>
                    </div>
                </div>

                <div>
                    <!--البوكس الثاني-->
                    <div>
                        <Button
                            class="{$page.url.pathname == '/' &&
                                'text-accent'} "
                            href="/"
                            variant="link"
                            style="text-decoration: underline;text-decoration-color:tomato;"
                        >
                            لأنك الله
                        </Button>
                    </div>
                    <div>
                        <Button
                            class="{$page.url.pathname == '/' &&
                                'text-accent'} "
                            href="/"
                            variant="link"
                            style="text-decoration: underline;text-decoration-color:tomato;"
                        >
                            الداء والدواء
                        </Button>
                    </div>
                    <div>
                        <Button
                            class="{$page.url.pathname == '/' &&
                                'text-accent'} "
                            href="/"
                            variant="link"
                            style="text-decoration: underline;text-decoration-color:tomato;"
                        >
                            رياض الصالحين
                        </Button>
                    </div>
                    <div>
                        <Button
                            class="{$page.url.pathname == '/' &&
                                'text-accent'} "
                            href="/"
                            variant="link"
                            style="text-decoration: underline;text-decoration-color:tomato;"
                        >
                            المنهاج من ميراث النبوة
                        </Button>
                    </div>
                </div>
            </div>
        </AboutCard>
    </div>

    <AboutCard>
        <div class="text-xl font-semibold text-center p-4">Rule in life :</div>
        <img src="/rule.png"/>

    </AboutCard>
</div>
