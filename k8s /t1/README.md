# Task 1 

## الهدف
- إنشاء Pod يشغل Nginx.
- تغيير البورت من 80 إلى 82 باستخدام ConfigMap.
- عمل Service من النوع ClusterIP عشان نقدر نوصله من باقي الـ Pods.
- عمل Curl على Pod IP و ClusterIP عشان نتأكد إنه شغال.


## الملفات
- **map-index.yaml** → configmap يعدل إعدادات Nginx عشان يشتغل على port 82.
- **index.yaml** → configmap للـ index.html (محتوى Welcome).
- **pod.yaml** → Pod يشغل Nginx ويربط الـ volumes مع الـ configmaps.
- **clusterip.yaml** → Service من النوع ClusterIP على port 82.
- **pod2.yaml** → Pod Nginx تاني للتست ونعمل curl منه على PodIP و ClusterIP.

---
