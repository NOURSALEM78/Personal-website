<script>
    import Container from "$lib/components/Container.svelte";
import ResumeCard from "$lib/components/ResumeCard.svelte";
import Title from "$lib/components/title.svelte";
</script>
<title>
    السيرة الذاتية
</title>
<Container>
        <Title title="السيرة الذاتية" ></Title>
    <div class="pt-16 flex flex-col gap-10">
        <div class="flex justify-between items-center">
            <spsn class="font-bold text-3xl"> التعليم والدورات</spsn>
        <!--<Button>تحميل السيرة الذاتية</Button>-->
        </div>
        <ResumeCard 
        date="2023 - Present" 
        title="علم بيانات" 
        company="جامعة أم القرى">
        </ResumeCard>
        <ResumeCard 
        date="2018 - (july 1 to 19)"
        title="Cryptology and Information Scurity"
        company="Mawhiba"
        >
            <p>برنامج حضوري تأسيسي في تشفير البيانات وحمايتها،</p>
            <p> تضمن عدة مهارات اساسية منها:  </p>
            <p>١-  القيادة والتأثير الاجتماعي<p/>
            <p>٢- التفكير الابداعي والابتكار</p>
            <p>٣- قيم المواطنة والاعتزاز بالشخصية الوطنية<p/>
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

        <div class="pt-16 flex flex-col gap-10">
            <spsn class="font-bold text-2xl">الخبرات</spsn>
            <ResumeCard
            date=""
            title="لا يوجد خبرات"
            company="">

            </ResumeCard>
            <div/>
        </div>
    </div>
</Container>