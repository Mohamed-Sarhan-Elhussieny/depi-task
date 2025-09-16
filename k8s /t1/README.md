# Task 1 

## الهدف
- إنشاء Pod يشغل Nginx.
- تغيير البورت من 80 إلى 82 باستخدام ConfigMap.
- عمل Service من النوع ClusterIP عشان نقدر نوصله من باقي الـ Pods.
- عمل Curl على Pod IP و ClusterIP عشان نتأكد إنه شغال.

## الملفات
- `configmap.yaml` → فيه إعدادات الـ nginx (listen 82 + index.html).
- `pod.yaml` → تعريف البود وربطه بالـ configmap.
- `service.yaml` → ClusterIP Service يوجّه الترافيك للـ Pod على بورت 82.
