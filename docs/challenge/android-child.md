---
layout: default
title: Android
parent: challenge 
---

# 마이그레이션
{: .no_toc .text-delta }

# 메모리 릭
{: .no_toc .text-delta }

---

## 마이그레이션(10 to 13)
- SplashScreen 실장방식의 변경
- android X를 실장하며 import package 변경
- PendingIntent 파라메터 종류 변경

## 메모리 릭
- largeHeap : 보통의 경우 태블릿에서 주로 쓰이는 옵션. 
- cursor변수를 try-with-resources로 변경.
- ? 계속 알람관계의 Activity가 메모리에 남았다고 LeakCanary로 부터 경고..
{: .no_toc }

## 어플 감시 서비스
- 스마트폰 부팅 중에 상태바를 내려오지 못하도록 제어하고 있었지만, 이것이 12부터 불가능하게 됨 (시스템 앱의 권한을 갖지 않는한)
{: .no_toc }
