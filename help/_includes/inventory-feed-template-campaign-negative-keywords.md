---
source-git-commit: 029e406fbfb4217ce78364c2d1f1a6dae24ff588
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 0%

---
# 텍스트 광고 템플릿 - 캠페인 수준 음성 키워드 설정

**[!UICONTROL Delete negative keywords when omitted from list]:**(Yandex를 제외한 모든 광고 네트워크, 선택 사항) 아래 목록에 지정되지 않은 템플릿을 사용하여 이전에 만든 기존 캠페인 수준의 부정적인 키워드를 삭제합니다. **참고:** 다른 방법(예: 일반 일괄 시트, [!UICONTROL Campaigns] 보기 또는 광고 네트워크의 광고 편집기에서)을 사용하여 만든 부정적 키워드는 템플릿을 사용하여 제거되지 않습니다.

**[!UICONTROL Set negative keywords by campaign name condition]:**(Yandex를 제외한 모든 광고 네트워크, 선택 사항) 이름에 지정된 문자열이 포함된 캠페인에 대해 부정적인 키워드를 지정할 수 있습니다. 이 옵션을 선택하면 최대 3개의 캠페인 이름 문자열과 해당 키워드를 추가할 수 있습니다.

각 문자열에 대해 **[!UICONTROL Add (Up to 3)]**&#x200B;을(를) 클릭하고 다음 정보를 입력합니다.

* **[!UICONTROL If campaign name contains]:** 캠페인 이름 내에서 찾을 텍스트 문자열입니다. 쿼리는 대/소문자를 구분합니다(예: &quot;[!DNL Car]&quot;이(가) 캠페인 이름 &quot;[!DNL Car Parts]&quot;과(와) 일치하지만 &quot;[!DNL INTERIOR CAR ACCESSORIES]&quot;은(는) 일치하지 않음).

* **[!UICONTROL Apply these negatives]:** 이름에 지정된 문자열이 포함된 캠페인에 추가할 정적 캠페인 수준의 부정적인 키워드입니다. 동일한 키워드에 대해 여러 키워드 또는 여러 일치 유형을 지정하려면 별도의 행에 입력합니다. 빼기 기호 없이 다음 구문을 사용합니다.

   * 음수 브로드 일치: `keyword`([!DNL Microsoft Advertising]에서 지원되지 않음)
   * 음수 구 일치: `"keyword"`
   * 정확히 일치하는 음수: `[keyword]`

구문과 정확한 일치 유형에 대한 일반적인 구문은 템플릿을 통해 피드 데이터를 전파할 때 생성되는 일괄 시트에서 사용됩니다. **참고:** [!UICONTROL Keywords] 탭이나 [!UICONTROL Search] > [!UICONTROL Campaigns] > [!UICONTROL Campaigns] 보기에서 음수 키워드를 볼 수 없습니다.

**[!UICONTROL All other campaigns: Apply these negatives]:**([!DNL Yandex]을(를) 제외한 모든 광고 네트워크; 선택 사항) 이름이 지정된 문자열과 일치하지 않는 캠페인에 추가할 정적 캠페인 수준의 부정적 키워드입니다. 동일한 키워드에 대해 여러 키워드 또는 여러 일치 유형을 지정하려면 별도의 행에 입력합니다. 빼기 기호 없이 다음 구문을 사용합니다.

* 음수 브로드 일치: `keyword`([!DNL Microsoft Advertising]에서 지원되지 않음)
* 음수 구 일치: `"keyword"`
* 정확히 일치하는 음수: `[keyword]`

구문과 정확한 일치 유형에 대한 일반적인 구문은 템플릿을 통해 피드 데이터를 전파할 때 생성되는 일괄 시트에서 사용됩니다. **참고:** [!UICONTROL Keywords] 탭이나 [!UICONTROL Search] > [!UICONTROL Campaigns] > [!UICONTROL Campaigns] 보기에서 음수 키워드를 볼 수 없습니다.
