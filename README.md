# autounattend-file
شرح الملف 📄❤️

كنت نزلت من فترة إن في إنجاز بسيط بخصوص نسخة ويندوز بتتسطب لوحدها، وناس كتير وقتها طلبت التفاصي فقولت أعمل البوست اللي بيشرح كله خطوة بخطوة.

الملف ده عبارة عن XML كود اسمه autounattend.xml بتخليه علي الفلاشة جمب     Setup.

هو المسؤول عن كل اللي بيحصل أوتوماتيك أثناء التثبيت، من أول ما الجهاز يعمل بوت من الفلاشة، لحد ما تفتح نسخة ويندوز جاهزة متزبطة على مزاجك.

الكود نفسه فيه  أجزاء لكل مرحلة من مراحل التثبيت، وكل جزء ليه وظيفة معينة

 وإن شاء الله هشرح كل جزئية فيه عشان تفهمها لو حبيت تعدل فيه برضو 

وكمان هقولك على ويب سايت تقدر من خلاله تعمل الملف ده تلقائي، وتختار كل الإعدادات اللي انت محتاجها وفي الاخر يعملك الملف دا .

  settings pass="windowsPE"> :  windowsPE - 1> في الكود

دي المرحلة الاولي اول ما الجهاز يبدا يعمل بووت من علي الفلاشة وكان من خلاله قدرت احدد اللغة والكيبورد واختار البارتشن ال هينزل عليه الويندوز واقسم الهارد وكنت حاطط فيه الاسكريبت بتاع التقسيم وف العادي ان ويندوز 11 بيطلب متطلبات تشغيل والكلام دا ف خلاني اتخطاها علطول.

 settings pass="specialize">  : Specialize - 2> 

 خاص بالتثبيت البرامج باسكربت باستخدام CMD  

 بتحدد المسار ال حاطط فيه البرنامج ال انت عايز تسطبه من الفلاشة وتضيفه في جزئية الكود دي

<RunSynchronousCommand wcm:action="add">

 <Path>C:\Windows\Setup\Scripts\ChromeStandaloneSetup64.exe /silent /install</Path>

</RunSynchronousCommand>

settings pass="oobeSystem"> : OobeSystem - 3>

عملت من خلاله يوزر ادمن واحد واديته الاسم وخلاني اتخطي اعدادات الشبكة مع صفحة الشروط وان اكسبتت وربط الجهاز مع حساب مايركروسوفت .

OfflineServicing - 4 :دي لو عايز تثبت تعريف او تحديث وقت تسطيب الويندوز بس بما ان نسختي نازلها بتعرفيتها فخلاص محتجتهاش.

 5- Extensions : دي استخدمتها عشان يظهرلي ايقونات الديسكتوب بدل ما ادخل اعدلها . 



 أنا ما كتبتش الكود كله بإيدي، لكن عدلت فيه حسب احتياجي، وكل مرة بأضيف حاجة بتسهل التثبيت أكتر وأكتر 🙌

 ولقيت موقع بيسهّل عليك الموضوع جدًا… تختار اللي انت عايزه وهو يطلعلك ملف جاهز:

🔗 https://schneegans.de/windows/unattend-generator/



ودا الفايل كنت شغال بيه بس خد بالك السكربت اللي استخدمته بيقسّم الهارد بالكامل وبيفرمته فلو هتستخدمه تأكد الأول من الباكاب.





في الآخر، شكرًا ليكو والله على دعمكم وكلامكم الجميل 💙

 ربنا يوفقكم كلكم، ولو حد محتاج أي مساعدة في إعداد نسخة بالشكل ده يبعتلي في أي وقت.

 

