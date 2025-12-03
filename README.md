# فارسی
---
#### ⚙️ آخرین تغییرات نسخه 2.5.9 - 03-12-2025
 - اکنون میتوانید گروه های کاربری و گروه های سرور را که در هیچ Authorization شرکت ندارند را مشاهده نمایید.
 - با کلیک روی هر سطر (یا کپس یکی از سلول های آن سطر) تمام آن ردیف Bold خواهد شد.
 - رنگ آمیزی زرد به Sub-protocols هر ردیف اضافه شد. اگر در یک ردیف Sub-protocols زرد مشاهده گردید، یعنی آن Sub-protocols به تارگت آن ردیف منتسب نشده ولی در آن Authorization برای حداقل یک تارگت دیگر استفاده میشود. 

---
#### ⚙️ آخرین تغییرات نسخه 2.5.6 - 30-11-2025
 - با کلیک روی آیتم های درون باکس های قسمت Ungrouped Entities و برخی سلول های جدول نهایی آیتم کلیک شده در کلیپ برد کپی خواهد شد. با نگه داشتن ماوس روی موارد قابل کپی، پیام مناسب نمایش داده خواهد شد.
 - موارد فیلتر شده در تمام باکس ها به ابتدای لیست مربوطه رفته و Sort میشود. 
 - برخی رنگ های با هدف تجربه کاربری بهتر، تغییر کرد.
---

#### ⚙️ آخرین تغییرات نسخه 2.5.3 - 25-11-2025
 - با کلیک روی آیتم های درون باکس های قسمت Ungrouped Entities آیتم کلیک شده در کلیپ برد کپی خواهد شد.پ
 - قابلیت جست و جو برای تمام باکس ها اضافه شد.
---
## 🌟معرفی
 برنامه **`SPA (Single-Page Application)`** ارائه شده در یک تک فایل **`HTML`** به صورت **`Offline`**. بدون نیاز به **`کتابخانه`**، **`وابستگی`** و **`نصب`**.
 
 با این برنامه می‌توانید تمام دسترسی‌های کاربران در سامانه WALLIX را با امکاناتی مانند فیلترسازی، مشاهده یا عدم مشاهده جزئیات ضروری و ... مشاهده نمایید.
 
 
## 🔑ویژگی‌های کلیدی
- کاملاً **`آفلاین`** 
- بدون نیاز به **`نصب`** 
- بدون نیاز به **`اینترنت`**  
- بدون نیاز به **`کتابخانه`**  
- ارائه شده در یک فایل **`HTML`**  
- قابل اجرا در تمام مرورگرهای مدرن  
- یکپارچگی کامل با CSV های Wallix

## 💎امکانات پیشرفته
- استفاده در دو مود، **`"کدام User به کدام Target دسترسی دارد؟"`** و **`"به کدام Target کدام User دسترسی دارد؟"`**  
- فیلترسازی اطلاعات بر اساس **`Authorization`**، **`IP`**، **`User`**، **`User Group`**، **`Target`**، و **`Target Group`**
- جدا سازی Targetهایی که هیچ User به آنها دسترسی ندارد  
- جدا سازی Userهایی که به هیچ Target دسترسی ندارند  
- نمایش ستون‌های مهم به صورت Optional  
- Sort چند لایه‌ای  
- تم Dark و Light  
- و بیشتر...

## 🛠️نحوه استفاده
> پیشنهاد می‌شود **`📖راهنمای کامل برنامه`** که در ادامه آمده است را مطالعه فرمایید.

 
1.در Wallix از منو سمت چپ وارد قسمت **`Import/Export → CSV`** بشوید.  

2.موارد زیر را تنظیم کنید:

🟥گزینه ![Field separator](https://img.shields.io/badge/-Field%20separator-ff0000?style=flat) را روی ![; (semicolon)](https://img.shields.io/badge/-%3B%20%28semicolon%29-007bff?style=flat) تنظیم کنید

🟥گزینه ![List separator](https://img.shields.io/badge/-List%20separator-ff0000?style=flat) را روی ![, (comma)](https://img.shields.io/badge/-%2C%20%28comma%29-007bff?style=flat)
 تنظیم کنید
  
  
3.گزینه‌های زیر را در قسمت Data انتخاب نمایید:  
- گزینه **`Authorizations`**
- گزینه **`Devices (or Resources or Targets)`**
- گزینه **`Target groups`**
- گزینه **`User groups`**
- گزینه **`Users`**  

4.روی **`Export`** کلیک کنید. 
 
5.فایل **`HTML`** برنامه را از اینجا دانلود و در یک مرورگر مدرن باز کنید.  

6.فایل **`zip`** دانلود شده در **`مرحله 4`** را از حالت فشرده خارج و با **`Drag and Drop`** به برنامه بدهید.

## ⚡راهنمای سریع
> پیشنهاد می‌شود **`📖راهنمای کامل برنامه`** که در ادامه آمده است را مطالعه فرمایید.

💬تعریف: **`دسترسی`** یعنی یک **`User Group`** با یک **`Target Group`** از طریق یک **`Authorization`** به یک دیگر متصل شده اند.

✅در نتیجه: تمام **`User`** های آن **`User Group`** به تمام **`Target`** های آن **`Target Group`** از طریق یک **`Authorization`** دسترسی خواهند داشت.


💬یادآوری: برای ایجاد یک دسترسی، **`User`** را عضو یک **`User Group`** می‌کنیم، **`Target`** را عضو یک **`Target Group`** می‌کنیم و این دو گروه را با یک **`Authorization`** به یکدیگر متصل می‌کنیم.

✅در نتیجه: پس در جدول نمایش داده شده هر **`ردیف`** به معنی یک اتصال بین یک **`User Group`** و یک **`Target Group`** از طریق یک **`Authorization`** است.

💡نکته: هنگام اضافه کردن یک **`Device`** می‌توان چندین پروتکل را تحت **`Service Name`** های مختلف به آن اعمال کرد. و هنگام اضافه کردن یک **`Device`** به یک **`Target Group`** مشخص می‌کنیم این **`Device`** با کدام **`Service Name`** های مجازش، به این **`Target Group`** اضافه شود، ولی لزوماً پروتکل‌های مجاز در **`Service Name`** برای این **`Device`** در این **`Target Group`**، در **`Authorization`** مجاز نخواهند بود.  

✨ مثلاً پروتکل نوع **`RDP`** را با **`Service Name`** انتخابی **`RDP-Jump`** به یک **`Device`** اعمال می‌کنیم و این **`Device`** را با همین پروتکل در یک **`Target Group`** اضافه می‌کنیم **`(Device:RDP-Jump)`**. ولی هنگام ایجاد دسترسی در قسمت **`Authorization`** برای این **`Target Group`** فقط پروتکل **`SSH`** را مجاز می‌کنیم. پس یک دسترسی ساخته‌ایم (چون یک **`User Group`** را به یک **`Target Group`** از طریق یک **`Authorization`** وصل کرده‌ایم) ولی پروتکل مجاز برای **`Device`** و پروتکل مجاز در **`Authorization`** با یکدیگر تطابق ندارند.  

با توجه به مثال بالا👇

در جدول نمایش داده شده، هر رنگ در ستون **`No`** معنی خاص خود را دارد:  
- 🟢رنگ سبز: تمام پروتکل‌های اعمال شده به یک **`Device`** که تحت یک **`Service Name`** در یک **`Target Group`** اضافه شده است، در **`Authorization`** این دسترسی مجاز است.  
- 🔴رنگ قرمز: تمام پروتکل‌های اعمال شده به یک **`Device`** که تحت یک **`Service Name`** در یک **`Target Group`** اضافه شده است، در **`Authorization`** این دسترسی غیرمجاز است.  
- 🟡رنگ زرد: برخی پروتکل‌های اعمال شده به یک **`Device`** که تحت یک **`Service Name`** در یک **`Target Group`** اضافه شده است، در **`Authorization`** این دسترسی مجاز است و برخی دیگر غیرمجاز است.

🔦با تیک زدن **`Sub-protocols`** از قسمت **`Optional Columns`** مشاهده خواهید کرد کدام دسترسی‌های منتسب به **`Device`** و **`Service`** آن که در **`Target Group`** آمده، در **`Authorization`** مجاز است **`سبز`** و کدام غیرمجاز **`قرمز`**.


## 📖راهنمای کامل برنامه  
💬تعریف: **`دسترسی`** یعنی یک **`User Group`** با یک **`Target Group`** از طریق یک **`Authorization`** به یک دیگر متصل شده اند.

✅در نتیجه: تمام **`User`** های آن **`User Group`** به تمام **`Target`** های آن **`Target Group`** از طریق یک **`Authorization`** دسترسی خواهند داشت.


💬یادآوری: برای ایجاد یک دسترسی، **`User`** را عضو یک **`User Group`** می‌کنیم، **`Target`** را عضو یک **`Target Group`** می‌کنیم و این دو گروه را با یک **`Authorization`** به یکدیگر متصل می‌کنیم.

✅در نتیجه: پس در جدول نمایش داده شده هر **`ردیف`** به معنی یک اتصال بین یک **`User Group`** و یک **`Target Group`** از طریق یک **`Authorization`** است.

💡نکته: هنگام اضافه کردن یک **`Device`** می‌توان چندین پروتکل را تحت **`Service Name`** های مختلف به آن اعمال کرد. و هنگام اضافه کردن یک **`Device`** به یک **`Target Group`** مشخص می‌کنیم این **`Device`** با کدام **`Service Name`** های مجازش، به این **`Target Group`** اضافه شود، ولی لزوماً پروتکل‌های مجاز در **`Service Name`** برای این **`Device`** در این **`Target Group`**، در **`Authorization`** مجاز نخواهند بود.  

### 📜راهنمای ابزار  
باکس ![View Settings](https://img.shields.io/badge/-View%20Settings-f27324?style=flat) 
> در این باکس می‌توانید جدول را مطابق نیازتان تغییر دهید.
- قسمت **`First Column`**: از این قسمت مشخص می‌کنید اولین ستون جدول **`User`** ها باشند یا **`Target`** ها. با توجه به انتخاب شما، فیلترسازهای جدول نیز با هدف تجربه کاربری بهتر، تغییر مکان می‌دهند😎
- قسمت **`Show Access Type`**: در این قسمت مشخص می‌کنید دسترسی از کدام نوع **`Account`** یا **`Scenario Account`** یا **`Account Mapping`** یا **`Interactive Login`** است. گزینه **`Integrated`** این اطلاعات را کنار نام سرور و گزینه **`Separate`** این اطلاعات را در یک ستون جدا نمایش خواهد داد. گزینه **`Hide`** نیز به‌طور کلی این اطلاعات را پنهان خواهد کرد. 
 - قسمت **`Show Service Name`**: در این قسمت مشخص می‌کنید در یک دسترسی (یک ردیف از جدول) کدام **`Service Name`** منتسب به **`Device`** دخیل است. گزینه **`Integrated`** این اطلاعات را کنار نام سرور و گزینه **`Separate`** این اطلاعات را در یک ستون جدا نمایش خواهد داد. گزینه **`Hide`** نیز به‌طور کلی این اطلاعات را پنهان خواهد کرد.  
💡نکته: اگر مرتب‌سازی را بر اساس این ستون‌ها انجام دهید، حتی اگر بعداً آن‌ها را مخفی کنید، باز هم مرتب‌سازی در جدول بر اساس این دو ستون اعمال خواهد شد و عدد لایه مرتب‌سازی نیز اینجا نمایش داده خواهد شد.  
- قسمت **`User Detail`**: در این قسمت می‌توانید مشخص کنید با نگه داشتن ماوس روی نام کاربران، اطلاعات مربوط به آنان نمایش داده شود یا نمایش داده نشود.

باکس ![Data Filters](https://img.shields.io/badge/-Data%20Filters-f27324?style=flat) 
> در این باکس می‌توانید جدول را بر اساس اطلاعات مورد نیاز خود فیلتر کنید.  
- کنار عنوان هر قسمت، تعداد کل آن نوع موجودیت نمایش داده می‌شود که اگر یک یا چند گزینه را انتخاب کنید، تعداد آن نیز نمایش داده خواهد شد.  
- اگر در قسمت **`Filter by Username`** مقدار **`No User in Group`** را دیدید، یعنی یک دسترسی (دسترسی چیست؟ اتصال یک **`User Group`** با یک **`Target Group`** از طریق یک **`Authorization`**) وجود دارد که هیچ **`User`** در **`User Group`** آن نیست.  
- اگر در قسمت **`Filter by Target/Resource`** مقدار **`No Target in Group`** را دیدید یعنی یک دسترسی (دسترسی چیست؟ اتصال یک **`User Group`** با یک **`Target Group`** از طریق یک **`Authorization`**) وجود دارد که هیچ **`Target`** در **`Target Group`** آن نیست.  
- اگر در قسمت **`Filter by Host IP`** مقدار **`No Host IP`** را دیدید یعنی یک دسترسی (دسترسی چیست؟ اتصال یک **`User Group`** با یک **`Target Group`** از طریق یک **`Authorization`**) وجود دارد که هیچ **`Target`** در **`Target Group`** آن نیست (بر اساس **`IP`** ها).

باکس ![Ungrouped Entities](https://img.shields.io/badge/-Ungrouped%20Entities-f27324?style=flat)
> در این باکس می‌توانید کاربرانی که به هیچ تارگتی دسترسی ندارند و تارگت هایی که هیچ کاربری به آن ها دسترسی ندارد (بر اساس نام+سرویس و بر اساس IP) مشاهده نمایید.
- قسمت **`Users without any access`** آن **`User`** هایی را نشان می‌دهد که هیچ دسترسی ندارند. یعنی فقط و دقیقاً یا در هیچ **`User Group`** عضو نیستند و یا اگر در **`User Group`** یا **`User Group`** هایی هستند، آن **`User Group`** ها در هیچ **`Authorization`** وجود ندارند. پس ممکن است کاربری باشد که هیچ دسترسی ندارد ولی چون در یک **`Authorization`** شرکت دارد، در اینجا نمایش داده نمی‌شود اما میتوانید برای یافتن چنین کاربرانی از قسمت **`Filter by Target/Resource`** گزینه **`No Target in Group`** و یا از قسمت **`Filter by Host IP`** گزینه **`No Host IP`** را انتخاب کنید.  
- قسمت **`Targets without any access`** آن **`Target`** هایی را نشان می‌دهد که هیچ **`User`** به آن ها دسترسی ندارد. یعنی فقط و دقیقاً یا در هیچ **`Target Group`** عضو نیستند و یا اگر در **`Target Group`** یا **`Target Group`** های عضو هستند، آن **`Target Group`** ‌ها در هیچ **`Authorization`** وجود ندارند. پس ممکن است **`Target`** باشد که هیچ **`User`** به آن دسترسی ندارد ولی چون در یک **`Authorization`** شرکت دارد، در اینجا نمایش داده نمی‌شود، اما مبتوانید برای یافتن چنین **`Target`** هایی از قسمت **`Filter by Username`** گزینه **`No User in Group`** را انتخاب کنید.  
قسمت **`Host IPs without any access`** مانند قسمت **`Targets without any access`** ولی بر اساس **`IP`**  
⁉️سوال: چگونه میتواند یک **`User`** در یک **`User Group`** باشد و آن گروه نیز در یک **`Authorization`** شرکت داشته باشد ولی به هیچ چیز دسترسی نداشته باشد؟  
پاسخ: یا **`Target Group`** این **`Authorization`** خالی است و یا **`Target`** های موجود در این **`Target Group`** سرویس های دارند (مثلا **`RDP`**) که در **`Authorization`** مجاز نیستند.  

باکس ![Optional Columns](https://img.shields.io/badge/-Optional%20Columns-f27324?style=flat)
> در این قسمت میتوانید ستون های اختیاری را جهت نمایش انتخاب نمایید.
در این باکس میتوانید مشخص کنید آیا یک دسترسی (یک ردیف در جدول):  
- آیا **`Recorded`** - ضبط میشود؟  
- آیا **`Critical`** - به عنوان یک دسترسی **`Critical`** علامت گذاری شده است؟  
- آیا **`Require approval`** - نیاز به تایید کاربر یا کاربرانی دارد؟  
- آیا **`Approver groups`** - اگر نیازمند تایید گروهی از کاربران است، آن گروه یا گروه ها کدام اند؟  
- آیا **`Approvers`** - اگر نیازمند تایید دیگران است، آن کاربریا کاربران کدام اند؟  
- آیا **`Sub-protocols`** -  پروتکل و زیر  پروتکل های مجاز در**`Authorization`** این دسترسی کدام است؟  
💡نکته: ممکن است برای یک دسترسی برخی پروتکل ها به **`Device`** اعمال شده باشد و در **`Target Gruop`** آن **`Device`** نیز انتخاب شده باشد ولی در **`Authorization`** مجاز نباشد. آن پرتکل هایی که هم به **`Device`** اعمال شده اند و هم در **`Target Group`** آن دیوایس انتخاب شده اند و هم در **`Authorization`** مجاز هستند، سبز بوده ولی آن پرتکل هایی که به **`Device`** اعمال شده اند و در **`Target Group`** آن **`Target`** نیز انتخاب شده اند ولی در **`Authorization`** مجاز نیستند، قرمز هستند!

### 📜راهنمای جدول  
هر ردیف از جدول یعنی یک دسترسی. هر دسترسی یعنی یک **`Authorization`** یک **`Usergroup`** و یک **`Targetgroup`** را به یکدیگر متصل کرده است. پس **`User`** های  آن **`User Group`** به **`Target`** های آن **`Target Group`** دسترسی خواهد داشت و تک به تک در ردیف های جدول نمایش داده خواهند شد.  
هدرهای جدول قابلیت مرتب سازی چند لایه دارند. یعنی میتوانید ابتدا بر اساس یک ستون، سپس بر اساس ستون دیگر و سپس بر اساس ستون بعدی و به همین صورت، جدول را **`Sort`** نمایید. شماره لایه هر ستون در مرتب سازی کنار آن نمایش داده میشود. همچنین کلیک اول، صعودی، کلیک دوم، نزولی و کلیک سوم آن ستون را از مرتب سازی خارج میکند.

رنگ ستون **`No`**  
در جدول نمایش داده شده، هر رنگ در ستون **`No`** معنی خاص خود را دارد:  
- رنگ سبز: تمام پروتکل‌های اعمال شده به یک **`Device`** که تحت یک **`Service`** در یک **`Target Group`** اضافه شده است، در **`Authorization`** این دسترسی مجاز است.  
- رنگ قرمز: تمام پروتکل‌های اعمال شده به یک **`Device`** که تحت یک **`Service`** در یک **`Target Group`** اضافه شده است، در **`Authorization`** این دسترسی غیرمجاز است.  
- رنگ زرد: برخی پروتکل‌های اعمال شده به یک **`Device`** که تحت یک **`Service`** در یک **`Target Group`** اضافه شده است، در **`Authorization`** این دسترسی مجاز است و برخی غیرمجاز است. با تیک زدن **`Sub-protocols`** از قسمت **`Optional Columns`** مشاهده خواهید کرد کدام دسترسی‌های منتسب به **`Device`** و **`Service`** آن که در **`Target Group`** آمده، در **`Authorization`** مجاز است **`سبز`** و کدام غیرمجاز **`قرمز`**.

  ## 📸تصاویر
![WABACL v2.5.0 (1)](./screenshots/WABACL-v2.5.0%20(1).png)

![WABACL v2.5.0 (1)](./screenshots/WABACL-v2.5.0%20(2).png)

![WABACL v2.5.0 (1)](./screenshots/WABACL-v2.5.0%20(3).png)

![WABACL v2.5.0 (1)](./screenshots/WABACL-v2.5.0%20(4).png)

![WABACL v2.5.0 (1)](./screenshots/WABACL-v2.5.0%20(5).png)

![WABACL v2.5.0 (1)](./screenshots/WABACL-v2.5.0%20(6).png)

![WABACL v2.5.0 (1)](./screenshots/WABACL-v2.5.0%20(7).png)

![WABACL v2.5.0 (1)](./screenshots/WABACL-v2.5.0%20(8).png)

---
# English
---


 #### ⚙️ Release Notes v2.5.6 - 30-11-2025
 - You can now view user groups and server groups that do not participate in any Authorization.
 - Clicking any row (or clicking one of that row's cells) will make the entire row **bold**.
 - Yellow highlighting was added to each row's Sub-protocols. If yellow Sub-protocols are seen in a row, it means those Sub-protocols are not assigned to that row's target but are used in that Authorization for at least one other target.
---
#### ⚙️ Release Notes v2.5.6 - 30-11-2025
- Clicking on items inside the Ungrouped Entities boxes and certain cells in the final table will copy the clicked item to the clipboard. When hovering over copyable items, an appropriate tooltip message will be displayed.

- Filtered items in all boxes are now moved to the top of their respective lists and sorted.

- Some colors have been updated to improve user experience.

---

#### ⚙️ Release Notes v2.5.3 - 25-11-2025
- Clicking on items inside the Ungrouped Entities boxes will copy the clicked item to the clipboard.

- Search functionality has been added for all boxes.

---
## 🌟Overview
The **`SPA (Single-Page Application)`** is provided as a single **`HTML`** file and works completely **`Offline`**. No **`libraries`**, **`dependencies`**, or **`installation`** are required.

With this application, you can view all user access permissions in the WALLIX system with features like filtering, showing or hiding essential details, and more.

## 🔑Key Features
- Fully **`Offline`**
- No **`Installation`** required
- No **`Internet`** required
- No **`Libraries`** required
- Delivered as a single **`HTML`** file
- Compatible with all modern browsers
- Full integration with Wallix CSV files

## 💎Advanced Features
- Operates in two modes: **`"Which User has access to which Target?"`** and **`"Which Target can be accessed by which User?"`**
- Filter data by **`Authorization`**, **`IP`**, **`User`**, **`User Group`**, **`Target`**, and **`Target Group`**
- Isolate Targets with no Users having access
- Isolate Users with no access to any Target
- Display important columns as Optional
- Multi-level Sorting
- Dark and Light Themes
- And more...

## 🛠️How to Use
> It is recommended to consult the **`📖Full Application Guide`** below.

1. In Wallix, navigate from the left menu to **`Import/Export → CSV`**.

2. Configure the following:

🟥Set the ![Field separator](https://img.shields.io/badge/-Field%20separator-ff0000?style=flat) to ![; (semicolon)](https://img.shields.io/badge/-%3B%20%28semicolon%29-007bff?style=flat)  

🟥Set the ![List separator](https://img.shields.io/badge/-List%20separator-ff0000?style=flat) to ![, (comma)](https://img.shields.io/badge/-%2C%20%28comma%29-007bff?style=flat)

3. Select the following options in the Data section:  
- **`Authorizations`**  
- **`Devices (or Resources or Targets)`**  
- **`Target groups`**  
- **`User groups`**  
- **`Users`**

4. Click **`Export`**.

5. Download the application's **`HTML`** file from here and open it in a modern browser.

6. Extract the **`zip`** file downloaded in **`Step 4`** and **Drag and Drop** it into the application.

## ⚡Quick Reference
> It is recommended to consult the **`📖Full Application Guide`** below.

💬Definition: **`Access`** means a **`User Group`** is connected to a **`Target Group`** via an **`Authorization`**.

✅Result: All **`Users`** of that **`User Group`** have access to all **`Targets`** of that **`Target Group`** via a single **`Authorization`**.

💬Reminder: To create access, assign a **`User`** to a **`User Group`**, a **`Target`** to a **`Target Group`**, and link the two groups with an **`Authorization`**.

✅Result: Therefore, each **`row`** in the table represents a connection between a **`User Group`** and a **`Target Group`** via an **`Authorization`**.

💡Note: When adding a **`Device`**, multiple protocols can be assigned under different **`Service Name`** entries. When adding a **`Device`** to a **`Target Group`**, specify which of its authorized **`Service Name`** entries are included, but the protocols allowed in the **`Service Name`** for this **`Device`** may not all be permitted in the **`Authorization`**.

✨Example: Apply the **`RDP`** protocol with **`Service Name`** `RDP-Jump` to a **`Device`**, and add this **`Device`** with the same protocol to a **`Target Group`** `(Device:RDP-Jump)`. When creating access in the **`Authorization`** section for this **`Target Group`**, only the **`SSH`** protocol is allowed. An access is created (linking a **`User Group`** to a **`Target Group`** via an **`Authorization`**), but the Device protocol and Authorization protocol do not match.

In the table, each color in the **`No`** column indicates:  
- 🟢Green: All protocols assigned to a **`Device`** under a **`Service Name`** in a **`Target Group`** are allowed in the **`Authorization`**.  
- 🔴Red: All protocols assigned to a **`Device`** under a **`Service Name`** in a **`Target Group`** are not allowed in the **`Authorization`**.  
- 🟡Yellow: Some protocols assigned to a **`Device`** under a **`Service Name`** in a **`Target Group`** are allowed in the **`Authorization`**, and some are not.

🔦By ticking **`Sub-protocols`** in **`Optional Columns`**, you can see which access permissions related to the **`Device`** and its **`Service`** in the **`Target Group`** are allowed **`green`** and which are not **`red`**.

## 📖Full Application Guide
💬Definition: **`Access`** means a **`User Group`** is connected to a **`Target Group`** via an **`Authorization`**.

✅Result: All **`Users`** of that **`User Group`** have access to all **`Targets`** of that **`Target Group`** via a single **`Authorization`**.

💬Reminder: To create access, assign a **`User`** to a **`User Group`**, a **`Target`** to a **`Target Group`**, and link the two groups with an **`Authorization`**.

✅Result: Therefore, each **`row`** in the table represents a connection between a **`User Group`** and a **`Target Group`** via an **`Authorization`**.

💡Note: When adding a **`Device`**, multiple protocols can be assigned under different **`Service Name`** entries. When adding a **`Device`** to a **`Target Group`**, specify which of its authorized **`Service Name`** entries are included, but the protocols allowed in the **`Service Name`** for this **`Device`** may not all be permitted in the **`Authorization`**.

### 📜Tool Guide
![View Settings](https://img.shields.io/badge/-View%20Settings-f27324?style=flat)  
> Use this section to adjust the table as needed.
- **`First Column`**: Choose whether the first column displays **`Users`** or **`Targets`**. Filter placements adjust accordingly for better UX 😎  
- **`Show Access Type`**: Select the type of **`Account`**, **`Scenario Account`**, **`Account Mapping`**, or **`Interactive Login`**. **`Integrated`** shows info next to the server name, **`Separate`** shows it in a separate column, **`Hide`** hides it completely.  
- **`Show Service Name`**: Determines which **`Service Name`** of a **`Device`** appears for a row. **`Integrated`** shows next to the server, **`Separate`** in a column, **`Hide`** hides it.  
💡Note: Sorting applied to these columns remains effective even if you hide them later; the sorting layer number is displayed.  
- **`User Detail`**: Hover over a username to view or hide additional info.

![Data Filters](https://img.shields.io/badge/-Data%20Filters-f27324?style=flat)  
> Filter the table based on your needs.  
- Next to each header, the total count of that entity type is displayed. Selecting options updates the counts.  
- **`Filter by Username`**: If **`No User in Group`** appears, it means a **`User Group`** has no users in this **`Authorization`**.  
- **`Filter by Target/Resource`**: If **`No Target in Group`** appears, the **`Target Group`** has no targets in this **`Authorization`**.  
- **`Filter by Host IP`**: If **`No Host IP`** appears, the **`Target Group`** has no targets with IPs in this **`Authorization`**.

![Ungrouped Entities](https://img.shields.io/badge/-Ungrouped%20Entities-f27324?style=flat)  
> View users with no access and targets with no users (by name+service or IP).  
- **`Users without any access`**: Shows users not in any **`User Group`**, or whose groups are not part of any **`Authorization`**.  
- **`Targets without any access`**: Shows targets not in any **`Target Group`**, or whose groups are not part of any **`Authorization`**.  
- **`Host IPs without any access`**: Same as above, based on IP.  
⁉️Question: How can a **`User`** be in a **`User Group`** that participates in an **`Authorization`**, yet have no access?  
Answer: Either the **`Target Group`** is empty or the targets have services (e.g., **`RDP`**) not allowed in the **`Authorization`**.

![Optional Columns](https://img.shields.io/badge/-Optional%20Columns-f27324?style=flat)  
> Select optional columns to display.  
For each row:  
- **`Recorded`** — is it recorded?  
- **`Critical`** — is it marked as **`Critical`**?  
- **`Require approval`** — requires approval from one or more users?  
- **`Approver groups`** — if group approval is needed, which groups?  
- **`Approvers`** — if approval by others is needed, which users?  
- **`Sub-protocols`** — which protocols and sub-protocols are allowed in the **`Authorization`**?  
💡Note: Some protocols may be applied to a **`Device`** and selected in a **`Target Group`**, but not allowed in the **`Authorization`**. Protocols applied to **`Device`**, in **`Target Group`**, and allowed in **`Authorization`** appear green; those not allowed appear red.

### 📜Table Guide
Each row represents an access — connecting an **`Authorization`**, a **`User Group`**, and a **`Target Group`**. Each **`User`** in the **`User Group`** has access to all **`Targets`** in the **`Target Group`**.  

Headers support multi-level sorting: sort by one column, then another, etc. The sorting layer number is displayed, click once for ascending, twice for descending, three times to remove sorting.  

**`No`** Column Colors:  
- Green: All protocols applied to a **`Device`** under a **`Service`** in a **`Target Group`** are allowed in **`Authorization`**.  
- Red: All protocols applied are not allowed.  
- Yellow: Some protocols are allowed, some are not. Ticking **`Sub-protocols`** in **`Optional Columns`** shows which are green and which are red.

  ## Screenshots
![WABACL v2.5.0 (1)](./screenshots/WABACL-v2.5.0%20(1).png)

![WABACL v2.5.0 (1)](./screenshots/WABACL-v2.5.0%20(2).png)

![WABACL v2.5.0 (1)](./screenshots/WABACL-v2.5.0%20(3).png)

![WABACL v2.5.0 (1)](./screenshots/WABACL-v2.5.0%20(4).png)

![WABACL v2.5.0 (1)](./screenshots/WABACL-v2.5.0%20(5).png)

![WABACL v2.5.0 (1)](./screenshots/WABACL-v2.5.0%20(6).png)

![WABACL v2.5.0 (1)](./screenshots/WABACL-v2.5.0%20(7).png)

![WABACL v2.5.0 (1)](./screenshots/WABACL-v2.5.0%20(8).png)
