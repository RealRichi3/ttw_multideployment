(r-code-reuse)=
# رمز قابل لإعادة الاستخدام
يمكن لمشروع البرنامج الخاص بك أن يتراوح بين برنامج نصي صغير تستخدمه في معالجة البيانات ودفتر ملاحظات يستخدم لتحليل البيانات، أو مكتبة برمجيات تنفذ الخوارزميات الخاصة بك. بغض النظر عن حجم أو صغر مشروع البرنامج الخاص بك، من المهم جعل التعليمات البرمجية الخاصة بك قابلة لإعادة الاستخدام.

ولأنواع مختلفة من البرمجيات متطلبات مختلفة لكي تكون قابلة لإعادة الاستخدام: لنص نصي صغير، وقد يكون الحصول على الوثائق الكافية كافيا، في حين قد يكون من الضروري إجراء اختبار شامل بالنسبة لمكتبة البرمجيات الحيوية للبعثة. في المستوى الأساسي جدا، كل ما عليك فعله هو وضع التعليمات البرمجية الخاصة بك على الإنترنت في مكان ما من المحتمل أن يستمر لفترة طويلة. نهج أكثر تفصيلاً لجعل برمجيات بحثك أكثر قابلية لإعادة الاستخدام هو باتباع مبادئ برامج البحث (FAIR Principles for Research Software (FAIR4RS) {cite:ps}`ChueHong2021FAIR4RS`.

عندما نتحدث عن جعل التعليمات البرمجية قابلة لإعادة الاستخدام، من المفيد توضيح ما نعنيه. في جدول تعاريف {ref}`للقابلية للتكاثر<rr-overview-definitions-reproducibility>` قمنا بتعريف البحث القابل للتكاثر على أنه استخدام نفس البيانات والشفرة نفسها. ومع ذلك، عندما نتحدث عن إعادة استخدام التعليمات البرمجية يمكن أن يأخذ هذا عدة أشكال: قد نريد تشغيل نفس التعليمات البرمجية بالضبط (بلغات البرمجة المجمعة). وهذا قد يعني حتى نفس الملف الثنائي) بالضبط، أو قد نرغب في تعديل شفرة المصدر وتوسيع نطاقها بطريقة معينة لتتناسب مع احتياجاتنا. Freire and Chirigati {cite:ps}`Freire2018Reduciity` يوفر إطاراً لمستويات مختلفة من القابلية للتكرار، اعتماداً على ما يمكن تعديله. وهي تحدد المستويات التالية من القابلية للتكرار: قابلة للتكرار، ويمكن إعادة تشغيلها، ويمكن تحويلها، ويمكن تمديدها، ويمكن تعديلها.

وبوسعنا أن نضع تعريفات لإطار فريري على النحو التالي:

| Freire framework | تعاريف التكرارية                                                          |
| ---------------- | ------------------------------------------------------------------------- |
| التكرار          | قابل للنسخ (نفس البيانات، نفس التحليل)                                    |
| إعادة التشغيل    | قوي & قابل للتكرار (نفس التعليمة البرمجية، بيانات مختلفة/تحليل/بارامترات) |
| محمول            | *لم يتم النظر في* (نفس الكود/البيانات، بيئة مختلفة)                       |
| قابل للتوسع      | (جزئيا) عامّ                                                              |
| قابل للتعديل     | (جزئيا) عامّ                                                              |

ولم يسبق النظر في إمكانية النقل بل في بيئة مختلفة للبرمجيات (مثل مختلف المعدات). وقد يؤثر نظام التشغيل أو حتى تركيب جديد على معدات مماثلة) على قدرة البرنامج على العمل (على سبيل المثال، قد يؤثر على التبعيات).

كما أن إمكانية التعميم تلخص مفهومين: القدرة الموسعة (القدرة على الاندماج مع برمجيات أخرى) والقدرة على التعديل (القدرة على تغيير جزء من التنفيذ لتوسيع نطاق وظيفتها).

في بقية هذا الفصل نقدم قائمة بالتوصيات التي يمكنك اتباعها للتأكد من أن الكود الخاص بك قابل لإعادة الاستخدام.