---
source-git-commit: 029e406fbfb4217ce78364c2d1f1a6dae24ff588
workflow-type: tm+mt
source-wordcount: '147'
ht-degree: 0%

---
# 계정 및 캠페인 설정의 추적 유형 필드

**[!UICONTROL Tracking Type]:** URL이 생성되는 메서드입니다.

* *[!UICONTROL EF Redirect]*(기본값): Adobe Advertising 전환 추적 서비스를 사용하려는 클라이언트의 경우. 이 방법은 고유한 클릭 추적 ID를 생성하고, 사용자를 클라이언트의 랜딩 페이지로 보내기 전에 추적 목적으로 Adobe Advertising 서버로 리디렉션합니다.

  이 메서드에는 선택적으로 사용자 지정할 수 있는 기본 추적 옵션이 있으며, 각 URL에 추가할 매개 변수를 지정할 수도 있습니다.

* *[!UICONTROL No EF Redirect]:* 자신의 클릭 추적 코드만 사용하려는 클라이언트의 경우 Search, Social 및 Commerce에서는 클릭 추적 ID 또는 리디렉션 코드를 제공하지 않습니다. 대상 URL이 있는 계정의 경우 각 대상 URL은 기본 URL과 동일합니다.

  **메모:**

   * 에이전시 계정 관리자, Adobe 계정 관리자 및 관리자 사용자만 이 값을 변경할 수 있습니다.
   * 추적 방법을 변경하는 경우 계정에 대한 추적 URL을 다시 생성해야 합니다.
   * 캠페인 수준 추적 옵션은 계정 수준 설정을 무시합니다.
