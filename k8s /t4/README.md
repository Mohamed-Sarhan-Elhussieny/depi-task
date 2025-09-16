Task 4: run two container into a pod 

  - البود فيه 2 كونتينر Nginx:
    - الكونتينر الأول → بيسمع على بورت 80 → بيعرض: `Welcome to pod 1`
    - الكونتينر التاني → بيسمع على بورت 50 → بيعرض: `Welcome to pod 2`
  - ConfigMaps مستخدمة علشان نعدل الـ `index.html` والـ `nginx.conf`
  - Service بيعمل  للبورتين (80 و 50) جوا الكلاستر
