# GitHub Upload Steps

## 1) داخل فولدر المشروع
```bash
git init
git add .
git commit -m "akma V2.03.13"
```

## 2) أضف الريموت
```bash
git remote add origin <YOUR_GITHUB_REPO_URL>
```

## 3) ارفع الفرع الرئيسي
```bash
git branch -M main
git push -u origin main
```

## 4) اعمل Tag للنسخة
```bash
git tag -a "akma-V2.03.13" -m "akma V2.03.13"
git push origin "akma-V2.03.13"
```

## 5) مع كل نسخة جديدة
```bash
git add .
git commit -m "akma V2.03.14"
git tag -a "akma-V2.03.14" -m "akma V2.03.14"
git push
git push origin "akma-V2.03.14"
```

## ملاحظة
استخدم دائمًا نفس نظام التسمية:
- اسم النسخة داخل المشروع: `akma V2.03.13`
- اسم الـ git tag: `akma-V2.03.13`
