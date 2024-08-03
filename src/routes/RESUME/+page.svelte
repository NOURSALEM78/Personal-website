<script>
import ResueCard from "$lib/components/ResueCard.svelte";
import Themeswitch from "$lib/components/Themeswitch.svelte";
import Button from "$lib/components/ui/button/button.svelte";
</script>
<title>
    السيرة الذاتية
</title>

<div class="max-w-screen-sm px-5 mx-auto py-12">
    <h1 class="mx-auto w-fit text-5xl font-bold flex items-center  ">
        <div class="bg-primary w-5 h-5 me-4"/>
        <span>السيرة الذاتية</span>
    </h1>
    <div class="pt-16 flex flex-col gap-10">
        <div class="flex justify-between items-center">
            <spsn class="font-bold text-2xl"> التعليم والدورات</spsn>
        <!--<Button>تحميل السيرة الذاتية</Button>-->
        </div>
        <ResueCard 
        date="٢٠٢٣-الان" 
        title="علم بيانات" 
        company="جامعة أم القرى">

        </ResueCard>
        <ResueCard 
        date="2018-(july 1 to 19)"
        title="Cryptology and Information Scurity"
        company="Mawhiba"
        >
        <p>
            برنامج حضوري تأسيسي في تشفير البيانات وحمايتها،</p>
            <p> 
                تضمن عدة مهارات اساسية منها:  </p>
                <p>١-  القيادة والتأثير الاجتماعي<p/>
                <p>٢- التفكير الابداعي والابتكار</p>
                <p>٣- قيم المواطنة والاعتزاز بالشخصية الوطنية<p/>
                <p></p>
        
        </ResueCard>
        <ResueCard
        date="19 jun-14 aug"
        title="Front-End developer"
        company="El-cato">
        <p>
            تتمحور الدورة حول لغات برمجة مثل HTML,CSS,JS,TS بالاضافة إلى إطار عمل 
            SvelteKit ومكتبة TailwindCSS وتغطي الدورة طريقة استضافة الموقع على رابط يمكن مشاركته 
        </p>
        </ResueCard>
        <div class="pt-16 flex flex-col gap-10">
            <spsn class="font-bold text-2xl">الخبرات</spsn>
            <ResueCard
            date=""
            title="لا يوجد خبرات"
            company="">

            </ResueCard>
            <div/>
        </div>
    </div>
</div>