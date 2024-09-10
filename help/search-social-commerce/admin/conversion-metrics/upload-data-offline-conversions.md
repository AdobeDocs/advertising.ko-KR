---
title: 향상된 전환을 위해 오프라인 전환 데이터 업로드
description: 자사 오프라인 전환 데이터를 업로드하여  [!DNL Google Ads] 향상된 잠재 고객 전환에 매핑하는 방법을 알아봅니다.
feature: Conversions
source-git-commit: c3cb1549adeb7b621c1b426c53da9bb09eddcbdc
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# 향상된 전환을 위해 오프라인 전환 데이터 업로드

*[!DNL Google Ads]개의 계정만*

<!-- Tweak metadata title/description and heading -->

해시된 이메일 주소와 전화 번호를 포함한 자사 오프라인 전환 데이터를 업로드하여 기존 [[!DNL Google Ads] 잠재 고객에 대한 향상된 전환](/help/search-social-commerce/admin/conversion-metrics/conversion-action-google.md)에 매핑할 수 있습니다. 업로드된 모든 데이터는 실시간으로 [!DNL Google Ads]에 동기화됩니다.

## 리드에 대한 [!DNL Google Ads] 향상된 전환에 대한 데이터 업로드

1. 주 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Admin] >[!UICONTROL Conversions]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Upload]** 탭을 클릭합니다.

1. 광고 네트워크를 선택한 다음 계정을 선택합니다.

1. (선택 사항) [!DNL Microsoft Excel] 형식의 모든 [필수 데이터 필드](#enhanced-conversions-leads-data)이(가) 있는 템플릿을 다운로드하려면 **[!UICONTROL View Template]**&#x200B;을(를) 클릭한 다음 브라우저의 일반 절차에 따라 파일을 다운로드하십시오.

   데이터를 포함하도록 파일을 편집하고 변경 사항을 저장한 다음 다음 단계에서 파일을 업로드할 수 있습니다.

1. **[!UICONTROL Choose File]**&#x200B;을(를) 클릭한 다음 장치 또는 네트워크에서 업로드할 파일을 선택하십시오.

## 업로드된 파일에 필요한 데이터 {#enhanced-conversions-leads-data}

### 테이블 위의 데이터

`Parameters:TimeZone=insert_timezone`

각 행에 대해 이 위치 또는 &quot;[!UICONTROL Conversion Time]&quot; 열에 계정의 시간대를 입력합니다. a) [지원되는 시간대 ID 형식](https://developers.google.com/google-ads/api/data/codes-formats#timezone_ids) 또는 b) + 또는 -로 표시된 GMT 오프셋과 4자리 시간 차이(예: 뉴욕의 경우 -0500)를 사용합니다.

### 테이블 열 및 값

| 열 | 설명 |
| ------ | ----------- |
| 이메일 | SHA-256 알고리즘을 사용하여 해시해야 하는 사용자의 이메일 주소. 각 행에는 이메일 값 또는 전화번호 값이 포함되어야 합니다. |
| 전화 번호 | SHA-256 알고리즘을 사용하여 해시해야 하는 사용자의 전화번호. 국가 코드가 포함되어야 하며 대시 및 기타 기호가 포함될 수 있습니다. 각 행에는 이메일 값 또는 전화번호 값이 포함되어야 합니다. |
| 전환 이름 | (필수) 전환 작업의 이름입니다. |
| 전환 시간 | (필수) 전환 이벤트가 [지원되는 시간 형식](https://support.google.com/google-ads/answer/7014069#prepare_data)에서 발생한 시간입니다. 데이터 테이블 위의 `Parameters:TimeZone=insert_timezone` 행에 계정의 시간대 ID를 포함하지 않는 경우 a) [지원되는 시간대 ID 형식](https://developers.google.com/google-ads/api/data/codes-formats#timezone_ids) 또는 b) + 또는 -로 표시된 GMT 오프셋과 4자리 시간 차이(예: 뉴욕의 경우 -0500)를 사용하여 각 행의 시간대를 포함합니다. |
| 전환 값 | (필수) 숫자 전환 값입니다. |
| 전환 통화 | 전환 이벤트에 대한 통화 코드입니다. |
| 광고 사용자 데이터 | (EEA(European Economic Area) 또는 영국(UK)의 사용자와 관련된 데이터에 적용 가능) 광고 개인화를 위해 [!DNL Google]에 사용자 데이터를 전송하는 데 동의했는지 여부를 나타냅니다. 값에는 `Granted`, `Denied` 또는 \[null\]([!DNL Google Ads]에 `Unspecified`(으)로 전송됨)이(가) 포함될 수 있습니다. **참고:** [!DNL Google Ads]은(는) 현재 잠재 고객의 향상된 전환에 대한 동의를 적용하지 않지만 향후 그렇게 할 수 있습니다. |
| 광고 Personalization | (EEA(European Economic Area) 또는 영국(UK)의 사용자와 관련된 데이터에 적용 가능) 광고 목적으로 [!DNL Google]에 사용자 데이터를 보내는 데 동의했는지 여부를 나타냅니다. 값에는 `Granted`, `Denied` 또는 \[null\]([!DNL Google Ads]에 `Unspecified`(으)로 전송됨)이(가) 포함될 수 있습니다. **참고:** [!DNL Google Ads]은(는) 현재 잠재 고객의 향상된 전환에 대한 동의를 적용하지 않지만 향후 그렇게 할 수 있습니다. |

>[!MORELIKETHIS]
>
>* [잠재 고객에 대한 전환 작업 만들기 [!DNL Google Ads] 향상된 전환](/help/search-social-commerce/admin/conversion-metrics/conversion-action-google.md)
>* [잠재 고객에 대한  [!DNL Google Ads] 향상된 전환 구현](/help/search-social-commerce/campaign-management/special-workflows/google-enhanced-conversions-leads.md)
>* [검색, 소셜 및 Commerce에서 추적한 전환 지표를  [!DNL Google Ads]](/help/search-social-commerce/tools/conversion-metrics-upload-to-google.md)에 업로드합니다.