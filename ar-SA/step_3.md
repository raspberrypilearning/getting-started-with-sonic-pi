## الأصوات الأولى مع Sonic Pi

![](images/GUI.png)

هذه هي واجهة Sonic Pi ، ولها ثلاث نوافذ رئيسية. أكبرها لكتابة التعليمات البرمجية الخاصة بك ، ونحن نسميها لوحة البرمجة. هناك أيضًا لوحة الإخراج التي تعرض معلومات حول برنامجك أثناء تشغيله. عند النقر فوق زر تعليمات ** ** في الجزء العلوي من النافذة ، تظهر اللوحة الثالثة على طول الجزء السفلي لعرض وثائق المساعدة. يحتوي هذا على معلومات حول التعليمات البرمجية المختلفة التي يمكنك تجربتها واستخدامها، بالإضافة إلى أصوات متزامنة مختلفة، وعينات وأكثر.

- تشغيل Sonic Pi من سطح المكتب أو قائمة التطبيقات.

- حدد ** المخزن المؤقت 1 ** واكتب:
    
    ```ruby
    عزف 60
    ```

- انقر على أيقونة **عزف ** في الجزء العلوي من الشاشة. ماذا حدث؟

- ماذا يحدث إذا كتبت ` pley 60 ` ونقرت على أيقونة عزف؟
    
    هذا مثال على خطأ في التعليمات البرمجية الخاصة بك. في الأنشطة اللاحقة، إذا كانت لوحة الخطأ تعرض نصًا ستعرف أن لديك خطأ تحتاج إلى إصلاحه. يمكن أن تكون قد أخطأت في تهجئة كلمة مثل ` عزف`.

- اكتب الآن:
    
    ```ruby
    عزف 60
    عزف 67
    عزف 69
    ```

- انقر على أيقونة عزف في الجزء العلوي من الشاشة. ماذا حدث؟

- يقوم الكمبيوتر بعزف كل النوتات بالتسلسل (واحدة تلو الأخرى)، ولكن يحدث بسرعة كبيرة لدرجة أنهم يبدوا كأنهم يعزفون بنفس الوقت.
    
    نحتاج إلى إخبار الكمبيوتر بالتوقف مؤقتًا بين النوتات. يمكننا القيام بذلك عن طريق كتابة ما يلي بعد كل `عزف `:
    
    ```ruby
    سكون 1
    ```
    
    القيمة التي تم إدخالها بعد كلمة `سكون` تمثل الوقت بالثواني. ويمثل استخدام القيمة 1 ثانية واحدة. ماذا ستكتب لمدة نصف ثانية؟

- الآن اكتب سلسلة من عزف وسكون لصنع نغمة رائعة!