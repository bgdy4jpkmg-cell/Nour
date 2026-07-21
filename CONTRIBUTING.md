# 🤝 دليل المساهمة

## شكراً لاهتمامك بالمساهمة في Nour! 🎉

هذا المستند يحتوي على إرشادات حول كيفية المساهمة في المشروع.

## قواعد السلوك 📋

المساهمون ملزمون بـ:
- احترام جميع أعضاء المجتمع
- عدم التمييز أو المضايقة
- الحفاظ على بيئة إيجابية

## خطوات المساهمة 🚀

### 1. Fork المشروع
```bash
git clone https://github.com/yourusername/Nour.git
cd Nour
```

### 2. إنشاء Branch جديد
```bash
git checkout -b feature/your-feature-name
# أو
git checkout -b fix/bug-name
```

### 3. قم بالتغييرات
- اتبع معايير الكود
- أضف اختبارات للميزات الجديدة
- اكتب commit messages واضحة

### 4. اختبر التغييرات
```bash
npm test
npm run lint
```

### 5. Push التغييرات
```bash
git push origin feature/your-feature-name
```

### 6. افتح Pull Request
- اكتب وصف واضح للتغييرات
- اربط أي issues ذات صلة
- اطلب مراجعة من المشرفين

## معايير الكود 📝

### JavaScript/React
```javascript
// ✅ جيد
const getUserProfile = async (userId) => {
  try {
    const response = await fetch(`/api/users/${userId}`);
    return await response.json();
  } catch (error) {
    console.error('Error fetching user:', error);
    throw error;
  }
};

// ❌ سيء
const getUserProfile = (userId) => {
  let data = fetch(`/api/users/${userId}`);
  return data;
};
```

### Commit Messages
```
✨ Add new feature description
🐛 Fix bug description
♻️ Refactor code
📝 Update documentation
🧪 Add tests
🎨 Improve UI/styling
⚡ Performance improvement
🔐 Security fix
🚀 Deploy changes
```

## اختبارات 🧪

كل PR يجب أن يحتوي على:
- Unit tests
- Integration tests (إن أمكن)
- اختبارات UI (للمكونات الجديدة)

```bash
# تشغيل الاختبارات
npm test

# التحقق من التغطية
npm run test:coverage
```

## التوثيق 📚

- اكتب توثيق واضح للدوال الجديدة
- أضف comments للكود المعقد
- حدّث README إذا لزم الأمر

## Issues 🔍

إذا وجدت مشكلة:
1. تحقق من أنها لم تُرفع من قبل
2. وفر وصف واضح
3. أضف أمثلة وخطوات التكرار
4. اذكر إصدار Node وOS

## الأسئلة الشائعة ❓

**س: كيف أبدأ؟**
ج: ابدأ بـ issues المعنونة "good first issue"

**س: كم وقت يستغرق review؟**
ج: عادة 2-5 أيام عمل

**س: هل يمكنني المساهمة من أي مكان؟**
ج: بالتأكيد! المساهمات موضع ترحيب من الجميع

## شكراً! 🙏

شكراً على مساهمتك في جعل Nour أفضل!
