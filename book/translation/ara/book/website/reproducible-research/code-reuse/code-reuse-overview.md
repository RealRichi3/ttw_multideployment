(r-code-reuse-recommendations)=
# نظرة عامة على إعادة استخدام الكود

يحتوي هذا القسم على قائمة مرجعية بالتوصيات لجعل برنامجك أكثر قابلية لإعادة الاستخدام. يحتوي قسم {ref}`rr-code reuse-detail` على شرح أكثر تعمقا لكل توصية من هذه التوصيات. يمكنك اتباع التوصيات الأكثر ملاءمة لنوع البرمجيات الخاص بك وتخطي تلك التي ليست ذات صلة في حالتك.

## التوصيات المتكررة

1. تأكد من أنك تستطيع العثور عليه (في الفضاء؛ معني: أن تكون قادراً على تحديد موقع المستودع/المشروع)
1. تأكد من أنك تستطيع العثور عليها (في الوقت؛ المعنى: أن تكون قادراً على تحديد موقع إصدار معين)
1. تأكد من أنك تستطيع تنفيذ نفس سلسلة العمليات
1. تأكد من أن بيئتكم وتسلسل عملياتكم قويين ولا حاجة إلى أي إنسان لتكرار ما تم إنجازه
1. رخصة الرمز الخاص بك
    - مع ترخيص يسمح بإعادة الاستخدام؛
    - مع رخصة متوافقة مع رخص التبعيات
1. تأكد من أنه قابل للكابل
1. تضمين البيانات الضرورية
1. كتابة وثائق مفيدة*

## توصيات قابلة لإعادة التشغيل

1. إزالة الأجزاء المقوى (مثل المسارات التي كانت موجودة فقط على القرص الصلب حيث تم تشغيل خط الأنابيب) وجعل الوحدة النمطية
1. اختبر أن الوحدات التي قمت بإنشائها يمكن أن تأخذ أنواعا مختلفة من بيانات الإدخال أو المعلمات
1. تحويل الوحدات إلى حزمة/صندوق أدوات
1. كتابة وثائق مفيدة*

## التوصيات المحمولة
1. تأكد من أنه يمكنك إعادة إنشاء البيئة حيث كانت تعيش
1. كتابة وثائق مفيدة*

## التوصيات الموسعة
1. كتابة وثائق مفيدة*

## توصيات قابلة للتعديل
1. تأكد من أن الكود الخاص بك مقروء من قبل البشر
1. تأكد من وجود التعليقات
1. كتابة وثائق مفيدة*

قد يلاحظ القارئ المراقب أن `كتابة وثائق مفيدة` مذكورة لكل مستوى من إعادة الاستخدام. ويرجع ذلك إلى الحاجة إلى مستويات مختلفة من الوثائق لمختلف مستويات إعادة الاستخدام.

## الوثائق

*الاحتياجات المختلفة من الوثائق لمختلف مستويات إعادة الاستخدام*

وكتابة الوثائق المفيدة شرط هام بالنسبة لجميع مستويات إعادة الاستخدام. غير أنه بالنسبة لمختلف مستويات إعادة الاستخدام، هناك احتياجات مختلفة من الوثائق:

الوثائق
- يشرح الاستخدام، محدداً:
  - ما الذي تفعله البرامج؛ (مطلوب للتكرار)
  - كيف يمكن استخدامها؛ (مطلوب للتكرار)
  - ما هي الخيارات/المعلمات المتاحة. (مطلوب للتكرار )
- يحتوي على أمثلة لكيفية تشغيله. (مطلوب للتكرار )
- لديه تعليمات التثبيت، بما في ذلك الأوصاف الجيدة لما يلي:
  - المعدات التي تعتمد عليها (على سبيل المثال GPUs)؛ (مطلوبة للأجهزة المحمولة)
  - • نظام التشغيل الذي تم اختبار البرمجيات عليه؛ (مطلوب للأجهزة المحمولة)
  - الاحتياجات من البرمجيات (مثل المكتبات والضوابط). (مطلوب للهاتف المحمول)