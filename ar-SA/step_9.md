## بث مباشر للتعليمات البرمجية!

تم تطوير Sonic Pi ليكون منصة للبرمجة الحية للموسيقى، بحيث يمكن التلاعب بالكود البرمجي وتغييره وتكييفه في الوقت الحقيقي؛ وهذا يعني أن المبرمجين يستطيعون تنفيذ تعليماتهم البرمجية بدلاً من تشغيل برامج مكتوبة مسبقاً. لماذا لا تنطلق؟

- في علامة تبويب جديدة للمخزن المؤقت:
    
    ```ruby
    define :play_my_synth do
      use_synth :prophet
      play 50, attack: 0.2, release: 1.3
      sleep 0.5
    end

    loop do
      play_my_synth
    end
    ```

- اضغط **عزف** لبدء البرنامج.

- بينما يتم عزف النغمة، علق على الخطوط الثلاثة الأخيرة بإضافة رمز `#` إلى بداية كل سطر مثل هذا:
    
    ```ruby
    # loop do
    # play_my_synth
    # end
    ```

- بعد ذلك قم بتغيير بعض التعليمات البرمجية في الدالة، واضغط على **عزف** مرة أخرى. أنت الآن متأرجح جدًا!