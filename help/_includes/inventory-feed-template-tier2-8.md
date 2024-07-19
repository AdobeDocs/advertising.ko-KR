---
source-git-commit: 029e406fbfb4217ce78364c2d1f1a6dae24ff588
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---
# 계층 2 - 쇼핑 광고 템플릿의 계층 8 필드

**[!UICONTROL Tier  2 - Tier 8]:**(제품 그룹의 계층을 추가할 때) 제품을 타겟팅할 제품 특성 유형과 선택한 특성 유형에 대한 자격 기준(예: Brand=Acme 또는 Condition=New)입니다. 값은 적격 제품을 결정하기 위해 계층적으로 적용됩니다. 속성 유형을 선택하고 자격 기준을 입력합니다. 금지된 문자는 템플릿의 열 이름, 템플릿의 수정자 이름 및 일괄 시트의 [!UICONTROL Parent Product Grouping] 열에 있는 계층 구분 기호를 지정하는 데 사용되는 `[ ] < > >>`(연속된 두 개의 &quot;보다 큼&quot; 기호)입니다.

&quot;[!UICONTROL All Products]&quot;(계층 1)을 포함하여 최대 8개의 제품 그룹 계층(수준)을 포함할 수 있습니다. 각 계층에는 여러 제품 그룹이 포함될 수 있지만, 동일한 속성 유형(예: &quot;조건&quot;)에 속해야 합니다.

>[!NOTE]
>
>* ([!DNL Google Ads]만 해당) [!UICONTROL Channel]에 대해 가능한 값은 &quot;[!UICONTROL Local]&quot; 또는 &quot;[!UICONTROL Online]&quot;이고 [!UICONTROL ChannelExclusivity]에 대해 가능한 값은 &quot;[!UICONTROL SingleChannel]&quot; 및 &quot;[!UICONTROL MultiChannel]&quot;입니다.&quot;
>* [!UICONTROL Search] > [!UICONTROL Campaigns] > [!UICONTROL Campaigns] 보기의 [!UICONTROL Product Groups] 탭에서 광고 그룹에 대한 두 번째 계층(하위) 제품 그룹을 만들 때 기본 광고 그룹 입찰을 사용하여 &quot;[!UICONTROL Everything Else]&quot;이라는 다른 제품 그룹이 자동으로 만들어집니다. 그러나 인벤토리 피드 템플릿을 사용하면 &quot;[!UICONTROL Everything Else]&quot; 제품 그룹이 제외됩니다.
>* 여러 계층을 포함하고 최종(번호가 가장 높은) 계층에 사용할 수 있는 값이 없는 경우 다음으로 높은 계층이 결합 가능한 제품 그룹으로 사용됩니다. 예를 들어 5개의 계층을 포함하고 계층 5에 사용할 수 있는 값이 없는 경우 계층 4가 결합 가능한 제품 그룹(단위)으로 사용됩니다. 그러나 중간 계층에 사용할 수 있는 값이 없으면 행이 무시됩니다. 예를 들어 5개의 계층을 포함하고 계층 5에는 값이 있지만 계층 4에는 값이 없는 경우 행 4는 무시됩니다.
