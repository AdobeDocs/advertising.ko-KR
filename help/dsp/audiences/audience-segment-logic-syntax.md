---
title: 대상 세그먼트 논리 구문
description: 대상 세그먼트에 대한 논리를 정의하는 데 사용할 수 있는 구문을 참조하십시오.
feature: DSP Audiences
exl-id: fb73f35f-1f65-463b-b93c-90804a8d19a9
TQID: 'https://experienceleague.adobe.com/FPci9npdKrFxwge6tw41Fhx4XAC9VqYFc-RZhLhILLo'
product_v2:
  - id: a829a185-511f-4bf8-8dcf-9e684f8011cf
    internal-label: Advertising
feature_v2:
  - id: ee30758d-9ffe-4cd7-8f26-0d4394f041f6
    internal-label: Demand Side Platform
  - id: b4dc2b3d-fdb5-55cd-9190-f1076d8563e4
    internal-label: DSP Audiences
subfeature_v2:
  - id: fef5c122-6482-4d17-a8ce-4e70b906f1f4
    internal-label: Audiences
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: 6d95caf72d11c404d866e8d091e1ffa89814ae73
workflow-type: tm+mt
source-wordcount: '142'
ht-degree: 0%
---
# 대상 세그먼트 논리 구문

재사용 가능한 대상을 만들 때 영숫자 세그먼트 ID(키)와 다음 구문을 사용하여 세그먼트 논리를 수동으로 정의할 수 있습니다.

* () 그룹을 나타냅니다.
* [!DNL OR] <!-- || escaped with backticks so Jenkins doesn't think it's a Markdown table -->에 대한 `||`
* [!DNL AND]에 대한 &amp;&amp;
* ! 대상: [!DNL NOT]&#x200B;(제외)

>[!NOTE]
>
>* 앞에 ! (이들 제외).
>* [!UICONTROL Audiences] > [!UICONTROL All audiences]에서 [대상자의 세그먼트 ID를 찾을 수 있습니다](reusable-audience-clipboard.md).

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
>* [대상자 관리 정보](audience-about.md)
>* [재사용 가능한 대상 만들기](reusable-audience-create.md)
>* [대상 설정](audience-settings.md)
>* [사용 가능한 타사 데이터 공급자](third-party-data-providers.md)
