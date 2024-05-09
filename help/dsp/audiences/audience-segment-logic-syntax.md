---
title: 대상 세그먼트 논리 구문
description: 대상 세그먼트에 대한 논리를 정의하는 데 사용할 수 있는 구문을 참조하십시오.
feature: DSP Audiences
exl-id: fb73f35f-1f65-463b-b93c-90804a8d19a9
source-git-commit: 4b9cc5956d573b346eacdf71a8ea490c162b4660
workflow-type: tm+mt
source-wordcount: '141'
ht-degree: 0%

---

# 대상 세그먼트 논리 구문

재사용 가능한 대상을 만들 때 영숫자 세그먼트 ID(키)와 다음 구문을 사용하여 세그먼트 논리를 수동으로 정의할 수 있습니다.

* () 그룹을 나타냅니다.
* `||` 대상 [!DNL OR] <!-- || escaped with backticks so Jenkins doesn't think it's a Markdown table -->
* &amp;&amp; [!DNL AND]
* ! 대상 [!DNL NOT] (제외)

>[!NOTE]
>
>* 앞에 ! (이들 제외).
>* 다음을 수행할 수 있습니다. [대상에 대한 세그먼트 ID 찾기](reusable-audience-clipboard.md) 출처: [!UICONTROL Audiences] > [!UICONTROL All audiences].

예를 들어, 다음 논리는

```
(X5vUk1cNvZxvBJ3jMjTt) || (sfvXrmQkk77PL5OtHpLH) && !(SMWSjTZFiy9hR1bKm1vw || x08UReA0IcP9HAJdcGVe)
```

수단(일반 영어)

```
[!DNL INCLUDE] Segment ID X5vUk1cNvZxvBJ3jMjTt [!DNL OR] INCLUDE Segment ID sfvXrmQkk77PL5OtHpLH [!DNL AND EXCLUDE] (Segment ID SMWSjTZFiy9hR1bKm1vw AND Segment ID x08UReA0IcP9HAJdcGVe)
```

>[!NOTE]
>
>배치 설정에서 저장된 대상을 명시적으로 타깃팅할 대상으로 사용하거나 타깃팅에서 제외할 별도의 대상으로 사용할 수 있습니다. 세그먼트 논리가 대상자 사용의 목적을 반영하는지 확인하십시오.

>[!MORELIKETHIS]
>
>* [재사용 가능한 대상의 세그먼트 키를 클립보드에 복사](reusable-audience-clipboard.md)
>* [대상자 관리 기본 정보](audience-about.md)
>* [재사용 가능한 대상 만들기](reusable-audience-create.md)
>* [대상자 설정](audience-settings.md)
>* [사용 가능한 타사 데이터 공급자](third-party-data-providers.md)
