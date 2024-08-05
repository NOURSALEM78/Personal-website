<script>
    import Container from "$lib/components/Container.svelte";
import ResumeCard from "$lib/components/ResumeCard.svelte";
import Title from "$lib/components/title.svelte";
import ResumeCard2 from "$lib/components/ResumeCard2.svelte";
</script>
<title>
    السيرة الذاتية
</title>
<Container class="">
        <Title title="السيرة الذاتية" ></Title>
    <div class="pt-16 flex flex-col gap-10">
        <div class="flex justify-between items-center">
            <spsn class="font-bold text-3xl dark:text-secondary"> التعليم والدورات</spsn>
        <!--<Button>تحميل السيرة الذاتية</Button>-->
        </div>
        <ResumeCard 
        date="2023 - Present" 
        title="علم بيانات" 
        company="جامعة أم القرى">
        <p>
            تخصص يدرس كيفية تتحول البيانات العملاقة
            إلى فرص ذهبية تساعد في صنع القرارات الحاسمة التي تؤثر 
            على مستقبل الشركات والمجتمعات، ويعلم الطلاب كيفية استخدام الأدوات 
            الإحصائية والبرمجية لاكتشاف الأنماط والتنبؤ بالاتجاهات.
        </p>
        </ResumeCard>
        <ResumeCard 
        date="2018 - (july 1 to 19)"
        title="Cryptology and Information Scurity"
        company="Mawhiba"
        >
        <p>برنامج حضوري تأسيسي في تشفير البيانات وحمايتها, تضمن عدة مهارات اساسية منها:</p>

        <ul class="list-decimal ps-4">
        <li>
        القيادة والتأثير الاجتماعي
        </li>
        <li>
        التفكير الابداعي والابتكار
        </li>
        <li>
        قيم المواطنة والاعتزاز بالشخصية الوطنية
        </li>
        </ul>
        </ResumeCard>

        <ResumeCard
        date="(19june to 14aug) - 2024"
        title="Front-End developer"
        company="El-cato">
        <p>
            تتمحور الدورة حول لغات برمجة مثل HTML,CSS,JS,TS بالاضافة إلى إطار عمل 
            SvelteKit ومكتبة TailwindCSS وتغطي الدورة طريقة استضافة الموقع على رابط يمكن مشاركته 
        </p>
        </ResumeCard>
        <div class="pt-8 flex flex-col gap-10">
            <spsn class="font-bold text-3xl dark:text-secondary">الخبرات والمهارات</spsn>
            <ResumeCard2
            title="الخبرات">
            <ul class="list-decimal ps-4">
            <li> منظم  </li>
            <li>مشرف تنظيم</li>
            <li>تصميم عروض وبوسترات </li>
            </ul>
            </ResumeCard2>
            
            <ResumeCard2 title="المهارات">
            <ul class="list-decimal ps-4">
            <li>اجادة استخدام كانفا</li>
            <li>التفكير الابداعي والابتكار</li> 
            <li>العمل الجماعي</li>
            <li>سرعة التعلم</li>
            <li>سرعة التعلم </li>          
            </ul>
            </ResumeCard2>
            <div/>
        </div>
    </div>
</Container>