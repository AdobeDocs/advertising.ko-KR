---
title: 사용자 관리
description: 방법 을 알아봅니다.
feature: Search Introduction
source-git-commit: 5a4c608d8c8371c24cf220cc5eed9a39989dc850
workflow-type: tm+mt
source-wordcount: '904'
ht-degree: 0%

---

# (새 UI) 검색, 소셜 및 상거래에 대한 사용자 관리

일부 사용자는 모든 Adobe 권한 및 사용자 관리를 관리하는 중앙 위치인 Adobe Admin Console을 사용하여 새로운 검색, 소셜 및 Commerce 사용자 인터페이스에 대한 액세스를 관리할 수 있습니다. 사용자는 최종 사용자 또는 관리자로 분류됩니다. 관리자인 경우 Adobe 계정 팀에서 알림을 보냅니다. 관리자인 경우 다음 섹션을 참조하여 사용자 관리를 위한 권한 및 워크플로를 식별하십시오.<!-- How can you see what your user role is, or will your Adobe Account Team tell you? -->

## 관리자 관련 유형

Admin Console은 여러 유형의 관리자를 제공하지만 검색, 소셜 및 Commerce과 관련된 관리자 유형 및 권한은 다음과 같습니다.

조직의 **시스템 관리자:** 수퍼 유저입니다. 시스템 관리자는 조직의 Admin Console에서 모든 관리 작업을 수행할 수 있으며 다른 사용자(제품 관리자)에게 관리 기능을 위임할 수 있습니다.&lt;!—, 제품 프로필 관리자 및 사용자 그룹 관리자  — 제품 관리자만 사용할 수 있다고 생각합니까?  확인합니다. —>

**제품 관리자:** 특정 [!DNL Adobe] 제품(예: Search, Social, Commerce)에 대한 액세스 권한과 해당 제품에 대한 사용자의 권한을 관리합니다. 제품 관리자는 제품에 대한 제품 프로필을 만들고, 사용자 및 사용자 그룹을 만들고(제거는 제외), 제품 프로필에서 사용자 및 사용자 그룹을 추가하거나 제거하고, 제품에서 다른 제품 관리자를 추가하거나 제거할 수 있습니다.

<!--
**Product profile admin:** Manages assigned product profiles for individual products. A product profile admin can add (but not remove) users and user groups to the organization; add or remove users and user groups from product profiles; and assign or revoke permissions from product profiles. [I don't think this is applicable: and manage the product roles for product profiles.]

**User group admin:** Manages assigned user groups and their access rights. A user group admin can add or remove users from groups and add or remove user group admins from groups.
-->

## 기본 제품 프로필

역할과 유사한 제품 프로필은 특정 제품에 대한 특정 서비스를 사용자에게 제공합니다.

검색, 소셜 및 상거래에 대한 새 사용자 인터페이스에는 다음과 같은 기본 제품 프로필이 있으며, 이러한 프로필은 다양한 기능 및 서비스 하위 집합을 제공합니다. 기본 제품 프로필을 편집하거나 삭제할 수 없습니다. 그러나 시스템 관리자는 필요에 따라 다른 권한 하위 집합으로 추가 제품 프로필을 만들고 관리할 수 있습니다.

* **기본 최적화:** 이 프로필은 다음 기능을 제공합니다.

   * 목표: 전체 액세스

   * 시뮬레이션: 전체 액세스

   * Portfolio 그룹: 전체 액세스

   * 포트폴리오: 목표, 캠페인 및 지출 관리에 대한 포트폴리오 설정에 대한 액세스 권한을 생성/편집하고 나머지 포트폴리오 설정에 대한 읽기 전용 액세스 권한을 부여합니다.

   * 캠페인: 캠페인 설정에 대한 읽기 전용 액세스(만들기, 편집 또는 삭제 기능을 사용할 수 없음), 제한 및 포트폴리오 할당에 대한 전체 액세스<!-- Is that the correct wording? -->

   * 광고 그룹: 광고 그룹 설정에 대한 읽기 전용 액세스(만들기, 편집 또는 삭제 기능을 사용할 수 없음), 제약 조건 및 포트폴리오 할당에 대한 전체 액세스<!-- Is that the correct wording? -->

  이 액세스 수준은 여전히 검색, 소셜 및 Commerce 사용을 학습하는 사용자에게 선호됩니다.

* **전문가 최적화:** 이 프로필은 다음 기능을 제공합니다.

   * 목표: 전체 액세스

   * 시뮬레이션: 전체 액세스

   * Portfolio 그룹: 전체 액세스

   * 포트폴리오: 전체 액세스

   * 캠페인: 캠페인 목록에 대한 읽기 전용 액세스(아직 캠페인 만들기, 편집 또는 삭제 기능을 사용할 수 없음), 제한 및 포트폴리오 할당에 대한 전체 액세스<!-- Is that the correct wording? -->

   * 광고 그룹: 광고 그룹 목록에 대한 읽기 전용 액세스(아직 캠페인 만들기, 편집 또는 삭제 기능을 사용할 수 없음), 제한 및 포트폴리오 할당에 대한 전체 액세스<!-- Is that the correct wording? -->

  이 액세스 수준은 검색, 소셜 및 Commerce의 전문가 사용자에게 권장됩니다.

* **읽기 전용:** 이 프로필은 다음 기능을 제공합니다.

   * 목표: 읽기 전용 액세스

   * 시뮬레이션: 읽기 전용 액세스

   * Portfolio 그룹: 읽기 전용 액세스

   * 포트폴리오: 읽기 전용 액세스

   * 캠페인: 읽기 전용 액세스

   * 광고 그룹: 읽기 전용 액세스

* **관리자:** 이 프로필은 사용 가능한 모든 기능에 대한 전체 액세스 권한을 부여하고 사용자가 새 클라이언트 인스턴스를 만들 수 있도록 합니다. 적절한 비즈니스 타당성이 없는 한 이 권한을 다른 사람에게 할당하지 마십시오.

<!-- Do I need to include this? If so, adjust wording as needed

## Product-specific instances

 -->

## 관리자용 작업

### Adobe Admin Console에 로그인하고 검색, 소셜 및 Commerce으로 엽니다

>[!PREREQUISITES]
>
>관리자 액세스 권한이 있어야 합니다.&lt;!어떤 종류요? 제품 관리자, 시스템 관리자이지만 제품 프로필 관리자 또는 사용자 그룹 관리자(내부 그룹 — check일 수 있음)도 Search, Social 및 Commerce에 있습니다 —>.

1. https://adminconsole.adobe.com/enterprise/으로 이동합니다.

1. (Experience Cloud에 로그인하지 않은 경우) Experience Cloud에 로그인합니다.

   1. [!DNL Adobe] ID를 입력하고 **[!UICONTROL Continue]**&#x200B;을(를) 클릭합니다.

   1. **[!UICONTROL Personal Account]&quot; 또는 &#x200B;** [!UICONTROL Company or School Account]**.<!-- Will it necessarily be "Company or School Account?" --> 중 하나를 선택하십시오.

   1. 해당 Experience Cloud 조직을 선택합니다.

   1. 제품 및 서비스에서 &quot;[!UICONTROL Adobe Advertising, Search, Social, & Commerce — Org Name]&quot;을(를) 클릭합니다.

   기본적으로 검색, 소셜 및 Commerce에 대한 [!UICONTROL Product profiles] 탭으로 제품 페이지가 열립니다. 추가 탭에는 [!UICONTROL Users] 및 [!UICONTROL Product Admins]이(가) 포함됩니다.

### 시스템 관리자를 위한 워크플로우

1. [Adobe Admin Console에 로그인하여 검색, 소셜 및 Commerce으로 열기](#open-admin-console).

1. [제품 관리자를 추가](https://helpx.adobe.com/kr/enterprise/using/admin-roles.html#enterprise)하여 제품 및 사용자 관리를 위임합니다.

<!-- what else? -->

### 제품 관리자를 위한 워크플로

1. [Adobe Admin Console에 로그인하여 검색, 소셜 및 Commerce으로 열기](#open-admin-console).

1. 필요에 따라 최종 사용자를 [개별적으로](https://helpx.adobe.com/kr/enterprise/using/manage-users-individually.html) 또는 [일괄적으로](https://helpx.adobe.com/kr/enterprise/using/bulk-upload-users.html)만드십시오.

1. (선택 사항) 각 제품 인스턴스에 대해 [사용자 그룹](https://helpx.adobe.com/kr/enterprise/using/user-groups.html)을(를) 만들고 각 사용자 그룹에 사용자를 할당합니다.

   인스턴스에 사용자가 많은 경우 사용자 그룹을 만들어 사용자가 전문 지식 수준에 따라 올바른 프로필이 할당되도록 합니다. (제품 프로필에 사용자 그룹을 할당하려면 4단계 를 참조하십시오.) LOB, 사용자 액세스 요구 사항, 사용자 고용 일자 또는 기타 기준에 따라 사용자 그룹을 생성할 수 있습니다.

   >[!IMPORTANT]
   >
   >사용자 그룹 이름은 사용자 그룹에 할당해야 하는 권한을 명확하게 전달해야 합니다. 예를 들어 &quot;읽기 전용&quot; 권한이 있는 사용자 그룹을 만들려면 사용자 그룹 이름에 &quot;Acme_Uk_ReadOnly&quot; 또는 &quot;Acme_ReadOnly&quot;와 같이 &quot;읽기 전용&quot;을 포함합니다.

1. (선택 사항) 정의된 권한 집합을 사용하여 [사용자 지정 제품 프로필을 만듭니다](https://helpx.adobe.com/kr/enterprise/using/manage-product-profiles.html).

   사용자 지정 프로필은 이미 사용 가능한 4개의 기본 제품 프로필에 추가됩니다.

   조직의 각 제품 프로필에는 고유한 이름이 있어야 합니다. 조직에서 여러 검색, 소셜 및 Commerce 인스턴스(예: Acme_US 및 Acme_JP)를 사용하는 경우 여러 인스턴스에서 제품 프로필 이름을 복제할 수 없습니다. **모범 사례:** &quot;Simulations_Only_JP&quot;와 같은 명명 규칙 `<Name>_<Instance>,`을(를) 사용합니다.

1. [각 사용자 또는 사용자 그룹을 관련 제품 프로필에 할당](https://helpx.adobe.com/kr/enterprise/using/manage-product-profiles.html)합니다. 수동으로 또는 일괄적으로.

## 전체 사용자 관리 안내서 및 추가 링크

* Adobe Admin Console을 사용한 사용자 관리에 대한 자세한 내용은 [Admin Console 개요](https://helpx.adobe.com/kr/enterprise/admin-guide.html)를 포함하여 &quot;[Adobe Enterprise &amp; Teams 관리 안내서](https://helpx.adobe.com/kr/enterprise/using/admin-console.html)&quot;을 참조하십시오.

* Admin Console: [https://adminconsole.adobe.com](https://adminconsole.adobe.com)
