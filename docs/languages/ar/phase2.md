# المرحلة 2 – البرمجة كائنية التوجه (2-3 أشهر)

## الفئات، الكائنات، السمات، والدوال
- هيكلية الفئة
- إنشاء الكائنات
- استخدام this
- أفضل الممارسات: التسمية، تنظيم الكود

## التغليف، الوراثة، التعددية، والتجريد
- **Encapsulation**: private, getters/setters, التحقق
- **Inheritance**: extends, overriding (@Override)
- **Polymorphism**: نوع فرعي، method overloading
- **Abstraction**: نظرة عامة، التحضير للـ interfaces والـ abstract classes

## الواجهات والفئات التجريدية
- **Interfaces**: implements, default methods
- **Abstract classes**: الدوال التجريدية والملموسة
- الفروق بين interface و abstract class

## المُنشئات، المُهيئات، والكتل الثابتة
- المُنشئات الافتراضية والمُمنهجة، الاستدعاء باستخدام this()
- كتل التهيئة ({}) والكتل الثابتة (static {})

## التعدادات
- إنشاء واستخدام enum
- الدوال والسمات في enums

## المجموعات الأساسية
- **ArrayList**: الإضافة، الحذف، التكرار (for, forEach, Iterator)
- **HashMap**: مفتاح-قيمة، العمليات الشائعة
- **HashSet**: إزالة التكرارات
- مقدمة إلى Queue و Stack (مثال: LinkedList كـ queue/stack)
- مقدمة إلى Java Collections Framework

## الخوارزميات الأساسية
- البحث الخطي والبحث الثنائي
- **Sorting**: Bubble Sort, Collections.sort()
- **Recursion**: المفاهيم وأمثلة بسيطة (مثال: العاملية، فيبوناتشي)
- مقدمة إلى التعقيد (O(n), O(log n))

## الجينيريكس
- الصيغة (<T>)، المجموعات الجينيريك، الدوال الجينيريك
- الحدود (extends, super)

## Stream API (مقدمة)
- **العمليات الأساسية**: filter, map, collect
- أمثلة مع ArrayList

## الاختبارات الوحدية (مقدمة)
- الاستخدام الأساسي لـ JUnit
- كتابة حالات الاختبار للفئات والدوال
- مقدمة إلى TDD (Test-Driven Development)

## المشروع النهائي
- **نظام المكتبة**
  - الفئات: Book, User, Library
  - الوراثة: DigitalBook و PhysicalBook
  - المجموعات: ArrayList للكتب، HashMap للإعارات
  - Encapsulation: التحقق من البيانات
- Git: commit لكل ميزة (مثال: `feature/book-management`)
- النشر على GitHub مع README توضيحي

## الموارد المحدثة
- [Oracle Java Tutorials (OOP)](https://docs.oracle.com/javase/tutorial/java/concepts/)
- [Baeldung Java OOP](https://www.baeldung.com/java-oop)
- [LeetCode](https://leetcode.com)
- [HackerRank](https://www.hackerrank.com)
- *Head First Java* (كتاب)
- [JUnit Tutorial Baeldung](https://www.baeldung.com/junit-5)
- [Khan Academy - Algorithms](https://www.khanacademy.org/computing/computer-science/algorithms)