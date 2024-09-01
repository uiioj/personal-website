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
            <div>Good luck! 🚀</div>
        </AboutCard>
    </div>
    <div>
        <AboutCard>
            <div class="text-xl font-semibold text-center">
                My book list :

            </div>

            <!--البوكس حق الكتب-->
            <div class="flex flex-col sm:flex-row justify-center items-center text-center">
                <div class="m-5">
                    <!--البوكس الاول-->

                    <div class="p-1">
                        <script lang="ts">
                            import * as Dialog from "$lib/components/ui/dialog";
                        </script>

                        <Dialog.Root>
                            <Dialog.Trigger
                                class="font-semibold"
                                style="text-decoration: underline;text-decoration-color:tomato;"
                                >سابغات</Dialog.Trigger
                            >
                            <Dialog.Content>
                                <Dialog.Header>
                                    <Dialog.Title class="text-center">
                                         سابغات 📙</Dialog.Title
                                    >
                                    <Dialog.Description class="text-center">
                                        الكتاب الجيد عملة صعبة، وبخاصة عندما
                                        تبحث فيه عن الجِدّة والمعاصرة، مع قوة
                                        المضمون، وجمال الأسلوب. هنا يمكن أن أقول
                                        مطمئناً: هذه عينة من العملة الكتابية
                                        الصعبة النادرة! إنه كتاب تمت هندسته بعد
                                        خبرة ميدانية معاصرة بواقع الشباب على
                                        اختلاف طبقاتهم وقضاياهم، وتوزيع
                                        جغرافيتهم، تلك الخبرة المتسمة باللقاءات
                                        وجهاً لوجه، المتصلة بعوالم الاتصالات
                                        الحديثة المسموعة والمرئية في حوارات
                                        متواصلة لا تكف عن الوعي وحسن الإرشاد
                                        والإقناع. كل ما مضى من الكتاب تمت صياغته
                                        بمنهج علمي وأسلوب عصري في اللغة وقرب
                                        صياغتها من واقع الأجيال
                                    </Dialog.Description>
                                </Dialog.Header>
                            </Dialog.Content>
                        </Dialog.Root>
                    </div>

                    <div class="p-1">
                        <script lang="ts">
                            import * as Dialog from "$lib/components/ui/dialog";
                        </script>

                        <Dialog.Root>
                            <Dialog.Trigger
                                class="font-semibold"
                                style="text-decoration: underline;text-decoration-color:tomato;"
                                >فاتتني صلاة</Dialog.Trigger
                            >
                            <Dialog.Content>
                                <Dialog.Header>
                                    <Dialog.Title class="text-center">
                                         فاتتني صلاة 📙</Dialog.Title
                                    >
                                    <Dialog.Description class="text-center">
                                        يتناول الكتاب كل الأفكار و الأعذار و
                                        الخواطر التي تختبيء داخل عقلك حول
                                        الصلاة، يمليها عليك كأنه أنت، كأنه يعرفك
                                        منذ زمن بعيد، يأخذ بيدك رفقاً ليخطوا بك
                                        داخل مملكة الصلاة
                                    </Dialog.Description>
                                </Dialog.Header>
                            </Dialog.Content>
                        </Dialog.Root>
                    </div>

                    <div class="p-1">
                        <script lang="ts">
                            import * as Dialog from "$lib/components/ui/dialog";
                        </script>

                        <Dialog.Root>
                            <Dialog.Trigger
                                class="font-semibold"
                                style="text-decoration: underline;text-decoration-color:tomato;"
                                >الحفرة السعيدة</Dialog.Trigger
                            >
                            <Dialog.Content>
                                <Dialog.Header>
                                    <Dialog.Title class="text-center">
                                         الحفرة السعيدة 📙</Dialog.Title
                                    >
                                    <Dialog.Description class="text-center">
                                        اعتدنا أن تكون الحُفر سقوطاً ونهايةً
                                        ووحشة،ماذا لو كانت تلك الحفرة رفعةً
                                        وخلوداً وجنة؟ ما ان انتهيت من صفحات
                                        الكتاب حتى استقر المعنى في نفسي ،أدركت
                                        ما يعنيه أن تكون أول منازل الآخرة بهذه
                                        الرقة ،وقلّما نجد وصفاً يليق بحفرة ،فكيف
                                        لو كان هو العنوان؟
                                    </Dialog.Description>
                                </Dialog.Header>
                            </Dialog.Content>
                        </Dialog.Root>
                    </div>
                    <div class="p-1">
                        <script lang="ts">
                            import * as Dialog from "$lib/components/ui/dialog";
                        </script>

                        <Dialog.Root>
                            <Dialog.Trigger
                                class="font-semibold"
                                style="text-decoration: underline;text-decoration-color:tomato;"
                                >فقه الأسماء الحسنى</Dialog.Trigger
                            >
                            <Dialog.Content>
                                <Dialog.Header>
                                    <Dialog.Title class="text-center">
                                         فقه الأسماء الحسنى 📙</Dialog.Title
                                    >
                                    <Dialog.Description class="text-center">
                                        رحلة إيمانية عميقة تغوص في أعماق المعاني
                                        العظيمة لأسماء الله الحسنى. يقدم الكتاب
                                        للقارئ فرصة فريدة للتدبر في هذه الأسماء
                                        وتأمل صفات الله تعالى. من خلال دراسة هذه
                                        الأسماء، يتقرب العبد من ربه ويعرف قدرته
                                        وعظمته، مما يزيد من إيمانه ويقينه
                                    </Dialog.Description>
                                </Dialog.Header>
                            </Dialog.Content>
                        </Dialog.Root>
                    </div>
                </div>

                <div class="m-5">
                    <!--البوكس الثاني-->

                    <div class="p-1">
                        <script lang="ts">
                            import * as Dialog from "$lib/components/ui/dialog";
                        </script>

                        <Dialog.Root>
                            <Dialog.Trigger
                                class="font-semibold"
                                style="text-decoration: underline;text-decoration-color:tomato;"
                                >لأنك الله</Dialog.Trigger
                            >
                            <Dialog.Content>
                                <Dialog.Header>
                                    <Dialog.Title class="text-center">
                                         لأنك الله 📙</Dialog.Title
                                    >
                                    <Dialog.Description class="text-center">
                                        رحلة استثنائية تأخذ القارئ في مغامرة
                                        روحانية عميقة لاستكشاف أسماء الله
                                        الحسنى. يهدف الكاتب إلى إيقاظ الإيمان
                                        الكامن في النفوس وإعادة صياغة العلاقة
                                        بين الإنسان وخالقه. من خلال تحليل معاني
                                        الأسماء الإلهية، يدعو القارئ إلى التعمق
                                        في صفات الله تعالى وتأملها في حياته
                                        اليومية. الكتاب لا يقتصر على الجانب
                                        النظري، بل يدعو القارئ إلى تطبيق هذه
                                        المعاني في حياته العملية، مما يساهم في
                                        تحقيق السعادة والسلام الداخلي
                                    </Dialog.Description>
                                </Dialog.Header>
                            </Dialog.Content>
                        </Dialog.Root>
                    </div>
                    <div class="p-1">
                        <script lang="ts">
                            import * as Dialog from "$lib/components/ui/dialog";
                        </script>

                        <Dialog.Root>
                            <Dialog.Trigger
                                class="font-semibold"
                                style="text-decoration: underline;text-decoration-color:tomato;"
                                >الداء والدواء</Dialog.Trigger
                            >
                            <Dialog.Content>
                                <Dialog.Header>
                                    <Dialog.Title class="text-center">
                                         الداء والدواء 📙</Dialog.Title
                                    >
                                    <Dialog.Description class="text-center">
                                        يعالج ابن القيم من خلال هذا الكتاب قضايا
                                        النفس البشرية وأدوارها، ورسم سبل إصلاحها
                                        وتزكيتها، فبين معنى المعصية وأسبابها
                                        وآثارها على النفس والمجتمع، ومآلاتها في
                                        الدنيا والآخرة، ثم عرض لبيان الدواء
                                        الناجح لهذا الداء، مستلهماً توجيهات
                                        القرآن الكريم والسنة النبوية في إصلاح
                                        النفوس والمجتمع. وقد اتسمت معالجته لهذا
                                        الموضوع بالدقة والموضوعية البالغة، فكان
                                        العالم الاجتماعي والمربي الحريص الذي
                                        يعرف مكنونات النفس البشرية وطبائعها
                                        وميولاتها، ويحدد أسباب الداء الذي
                                        أصابها، ثم يشرع في وصف الدواء الملائم من
                                        خلال أحكام الشريعة وفضائها
                                    </Dialog.Description>
                                </Dialog.Header>
                            </Dialog.Content>
                        </Dialog.Root>
                    </div>
                    <div class="p-1">
                        <script lang="ts">
                            import * as Dialog from "$lib/components/ui/dialog";
                        </script>

                        <Dialog.Root>
                            <Dialog.Trigger
                                class="font-semibold"
                                style="text-decoration: underline;text-decoration-color:tomato;"
                                >رياض الصالحين</Dialog.Trigger
                            >
                            <Dialog.Content>
                                <Dialog.Header>
                                    <Dialog.Title class="text-center">
                                         رياض الصالحين 📙</Dialog.Title
                                    >
                                    <Dialog.Description class="text-center">
                                        خيرٌ رفيق كلام خير الأنام ﷺ، كتاب يعرفك
                                        على مرامي الرعيل الأول ويأخذك إلى رِياض
                                        قلوبهم لتحظى بالاقتداء وتَّأنس هو ليس
                                        كتاب بل هو مرشد للحياة وأي حياة؟ مخضرة
                                        عذبة حلوة ترى من خلالها الحقيقة. يكفيك
                                        أن تقرأ كلام خرج من فيه ﷺ كلامه يؤدبك في
                                        مطعمك ،ومشربك، ونومك وكل تفاصيل حياتك
                                        لتمسك بيدك وترى بقلبك حبل النور الموصل
                                        لسماء وترقى حتى تصل للحياة الحقيقة
                                    </Dialog.Description>
                                </Dialog.Header>
                            </Dialog.Content>
                        </Dialog.Root>
                    </div>
                    <div class="p-1">
                        <script lang="ts">
                            import * as Dialog from "$lib/components/ui/dialog";
                        </script>

                        <Dialog.Root>
                            <Dialog.Trigger
                                class="font-semibold"
                                style="text-decoration: underline;text-decoration-color:tomato;"
                                >المنهاج من ميراث النبوة</Dialog.Trigger
                            >
                            <Dialog.Content>
                                <Dialog.Header>
                                    <Dialog.Title class="text-center">
                                         المنهاج من ميراث النبوة 📙</Dialog.Title
                                    >
                                    <Dialog.Description class="text-center">
                                        الكتاب يفتح بعض الأبواب المضيئة في
                                        القرآن والسنة التي يحتاجها كل مسلم مؤمن
                                        في حياته وعمله وقوله وفعله، آيات تلامس
                                        القلب وتحرك الوجدان، وأحاديث تخاطب العقل
                                        وتحاكي النفس. الكتاب عدة أبواب ومنها
                                        الصدق والنية والفتن والعمل، وكل آية
                                        وحديث في موضعهما المناسبين الذين يدعمان
                                        عنوان الباب
                                    </Dialog.Description>
                                </Dialog.Header>
                            </Dialog.Content>
                        </Dialog.Root>
                    </div>
                </div>
            </div>
        </AboutCard>
    </div>

    <AboutCard>
        <div class="text-xl font-semibold text-center mb-7">Rule in life :</div>
        <img src="/rule.png" />
    </AboutCard>
</div>
