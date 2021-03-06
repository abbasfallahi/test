  
#### Abbas Fallahi         
  
ID: 99210572
  
#### 1:
  
  
افشای اطلاعات سازمان از طریق فلش مموری از جمله تهدیدات داخل سازمانی است، که توسط افراد سازمان به صورت عمدی یا غیرعمدی می تواند انجام شود. ابتدا به افشای اطلاعات به صورت غیر عمدی می پردازیم
فرض کنید کارکنان سازمان فلش مموری حاوی بدافزاری را پیدا می کنند و برای تشخیص صاحب فلش آن را به سیستم سازمان متصل می کنند، در نتیجه اطلاعات سازمان از طریق بدافزار برای صاحب فلش مموری ارسال می شود. این نفوذ در سال 2008 علیه پایگاه نظامی ایالات متحده در خاورمیانه اتفاق افتاد، که در نهایت پنتاگون استفاده از وسایل جانبی از قبیل فلش مموری را ممنوع کرد. اما در نفوذ عمدی کارکنان سازمان به دلایل مختلف مالی، فروش اطلاعات محرمانه، نارضایتی و ... با استفاده از فلش مموری اطلاعات سازمان را استخراج می کنند و در دسترس سازمان های رقیب و حتی عموم قرار میدهند
  
در سناریوی ذکرشده که از جمله تهدیدات درون سازمانی عمدی است، کارکنان با استفاده از فلش مموری اطلاعات سازمان را استخراج می کنند و در نهایت اطلاعات را در سایت ویکی لیکس (با هدف افشای اطلاعات برای عموم) آپلود می کنند. این آپلود میتواند با هدف مالی و یا فقط ضربه زدن به سازمان انجام شود
  
  
##### برای جلوگیری از این سناریو می توان به موارد زیر اشاره کرد:
  
1:استفاده از فلش مموری و هر گونه دستگاه رسانه ای قابل جابه جایی ممنوع شود
2:زمان انتقال اطلاعات به فلش مموری، اطلاعات به صورت خودکار توسط سیستم رمزنگاری شود 
3:استفاده از زیرساخت دسکتاپ مجازی __---> Virtual Desktop Infrastructure__
در این حالت دسکتاپ کارکنان در ماشین مجازی اجرا شده و در نهایت از طریق شبکه به کاربر نهایی می رسند. بنابراین همه داده ها در سرور ذخیره می شوند و نه در کاربر نهایی. پس کارکنان نمی توانند هر فایلی را دانلود و یا کپی کنند.
  
[VDI-PIC](https://s18.picofile.com/file/8432628134/Virtual_Desktop_Infrastructure.png )
  
4: نظارت بر فعالیت کاربر __---> User Activity Monitoring__
گاهی کارمند از ابتدا قصد انجام این سناریو را ندارد و به دلایلی در جریان سازمان ممکن است، دست به چنین عملی بزند. با شناسایی رفتار مشکوک کارمندان می توان تا حدی سوءقصد افراد را شناسایی کرد.
  
5: مدیریت حقوق دیجیتال __---> DRM__
بد نیست اشاره ای به مدیریت حقوق دیجیتال به عنوان راهکاری برای جلوگیری از  نشت اطلاعات 
دیجیتالی داشته باشیم.(اطلاعات سازمان ممکن است، کتاب های الکترونیکی و ... باشد)
  
##### قابل اجرا بودن راهکارها:
  
با توجه به اینکه کارکنان سازمان به عنوان افراد مورد اعتماد، در سازمان شناخته می شوند، پس جلوگیری از انجام سناریو ذکر شده به طور کامل قابل انجام نیست. ولی میتوان با پروفایل کردن رفتار کارکنان تا حدی از سوء قصد افراد نسبت به اطلاعات جلوگیری کرد. همچنین پروسه رمزنگاری ممکن است، بسته به نوع رمزنگاری سربار پردازشی داشته باشد و یا در نهایت اطلاعات رمزگشایی شوند. استفاده از زیرساخت دسکتاپ مجازی ایده خوبی است و میتوان با ارتقا سطح امنیتی از انجام سناریو جلوگیری کرد.
  
[Reference](https://www.mdpi.com/2079-9292/9/9/1460/pdf )
  
  
##### بررسی و تحلیل داده ها:
  
با اجرای فایل مربوط به سناریو فوق می توان به 3 مورد مشکوک رسید. فرد مخرب ایتدا به سیستم لاگین کرده، سپس به دیوایس (از طریق فلش مموری) متصل شده است و در نهایت اطلاعات استخراج شده را در سایت ویکی لیکس آپلود کرده است.
  
file ---> r3.1-1.csv
[scenario-1-PIC](https://s18.picofile.com/file/8432672418/exfiltration_attack.png )
  
#### 2:
  
سیستم یا داده های کارکنان در سازمان باید در مقابل افراد دیگر سازمان حفاظت شود. زیرا یک خودی مخرب یا کارمند ناراضی از طریق نفوذ به سیستم های کارکنان با هدف صدمه زدن به سازمان، افراد و یا مجازات کارفرمای خود به سرقت اطلاعات و اختلال در عملیات سازمان می پردازد.
 بنابراین اگر اطلاعات افراد سازمان به صورت ایزوله محافظت نشود، خودی مخرب می تواند بسیار خطرناک باشد. اقدامات عملیاتی خودی مخرب می تواند، شامل تزریق بدافزار به سیستم ها، سرقت اطلاعات محرمانه افراد بالا دست خود، آسیب رساندن به داده ها و ... باشد.
  
سناریو دوم به خودی مخربی در سازمان اشاره می کند که با هدف استخدام در سازمان رقیب در پستی بهتر از شرایط فعلی، اطلاعات محرمانه سازمان را از سیستم های افراد با درجه پستی بالاتر دزدیده و در جهت رسیدن به هدف خود به سازمان رقیب تحویل می دهد.
  
#####  بررسی و تحلیل داده ها:
  
در این سناریو، فرد مخرب ابتدا به سایت های مختلف سر می زند و با سایت __لاک هید__ ارتباط برقرار می کند.. این ارتباط از طریق ایمیل شروع می شود و سازمان رقیب (لاک هید) به فرد پیشنهاد استخدام به عنوان مدیر با حقوق خوب را می دهد. همه این موارد در ایمیل ها دیده می شود. همچنین در ایمیل ها از جاسوسی، تخلف، صاحب سهام صحبت شده است. با توجه با این کلمات کلیدی می توان دریافت که فرد در ازای جاسوسی در سازمان فعلی، در سازمان رقیب استخدام می شود. پس از اتمام گفت و گو ها در نهایت فرد به مدیر سازمان فعلی ایمیل می زند و اعلام استعفا می کند.
  
##### مراحل تحلیل:
  
1: مشخص شدن جسجتوی فرد برای کار و در نهایت ارتباط با سایت لاک هید از طریق ایمیل
[1-pic](https://s18.picofile.com/file/8432674250/lockheed.png )
  
2: ذخیره محتوای پیام ها
[2-pic](https://s19.picofile.com/file/8432674584/save_emails.png )
  
3: یافتن کلمات کلیدی که در نهایت با کلمات زیر مواجه شدم
[3-pic](https://s19.picofile.com/file/8432675218/words.png )
 Spion = جاسوسی
 Counterspy = متخلف
 Share owner = صاحب سهام
 Grand partners = شرکای بزرگ
 Management experience = تجربه مدیریت 
 Recruit = استخدام
 Resign = استعفا دادن
از کلمات فوق می توان دریافت که استخدام در ازای جاسوسی انجام می شود.
  
4: بررسی ارسال ایمیل نهایی فرد به اعضای شرکت.دریافت کننده ایمیل مدیر شرکت فعلی بوده است و اینکه در محتوای ایمیل فرد استعفا می دهد.
[4-pic](https://s18.picofile.com/file/8432676184/malicious.png )
  
#### 3:
  
  
با توجه به مقالاتی که مطالعه کرده ام. برای تشخیص و بررسی سناریوهای احتمالی حمله می توان از مدل گراف رابطه ای استفاده کرد. گرافی که نشان دهنده ی شبکه رابطه ای واقعی درون سازمان است.
این گراف از ارتباط چندین مدل و گراف مختلف تشکیل شده است، که هر کدام با توجه به داده های مورد نظر نوعی از رفتار سازمانی را مدل می کنند. در نهایت با استفاده از الگوریتم های آنالیز داده، گراف های رفتاری با رفتار فعلی کاربر مقایسه می شود و با توجه به مقیاس های ارزیابی، رفتار احتمالی حمله تشخیص داده می شود.
  
##### داده های مورد بررسی:
  
##### داده های قاطع:
  
فرکانس شمارش در مکان هایی که کاربر لاگین کرده است
برنامه هایی که کاربر به آنها وارد شده است
دستورات و عملیات اجرا شده
  
##### داده های عددی:
  
تعداد بایت های منتقل شده از طریق اف تی پی
تعداد ایمیل های ارسال شده
مدت زمان بین ورود و خروج کاربر از سیستم
تعداد سرورهای دسترسی یافته در 1 روز
  
##### داده های زمانی:
  
ساعت ها و روزهایی که کاربر به وی پی ان متصل می شود.
زمانی که کاربر وارد ساختمان می شود
زمانی که کاربر فعالیت فایلی دارد
  
[Date-Type-PIC](https://s19.picofile.com/file/8432645484/data_type.png )
  
[Reference-1](https://www.exabeam.com/wp-content/uploads/2019/04/Lin-Insider-Threat-Detection.pdf )
[Reference-2](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=6565236 )
  
#####  دقت در داده ها:
  
1:نیاز به منبع برچسب گذاری برای تشخیص کلمات مرتبط با موضوعات نامگذاری شده
2: نشان دادن اهمیت کلمات بااستفاده از روش های آماری و وزن دهی __--> tf.idf__
  
  
### 
  
  