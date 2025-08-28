---
source-git-commit: 47b5d399d4a5daa8832456abc32fff68e694abe9
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 0%

---
# Adobe Advertising

## Adobe Advertising

EF ID는 Adobe Advertising이 활동을 온라인 클릭 또는 광고 노출과 연결하는 데 사용하는 고유한 토큰입니다. EF ID는 [an [!DNL Analytics] [!DNL eVar]](https://experienceleague.adobe.com/docs/analytics/components/dimensions/evar.html?lang=ko) 또는 [!DNL rVar]&#x200B;(예약된 [!DNL eVar]) 차원(Adobe Advertising EF ID)에 저장되며 개별 브라우저 또는 장치 수준에서 각 광고 클릭 또는 노출을 추적합니다. EF ID는 주로 Adobe Advertising 내에서 보고 및 입찰 최적화를 위해 [!DNL Analytics] 데이터를 Adobe Advertising에 보내는 키 역할을 합니다.

### EF ID 형식 {#ef-id-formats}

>[!NOTE]
>
>EF ID는 대/소문자를 구분합니다. [!DNL Analytics] 구현에서 URL 추적을 소문자로 강제하는 경우 Adobe Advertising에서 EF ID를 인식하지 못합니다. 이는 Adobe Advertising 입찰 및 보고에 영향을 주지만 [!DNL Analytics] 내의 Adobe Advertising 보고에는 영향을 주지 않습니다.

#### [!DNL Google Ads]개 검색 광고

```
{gclid}:G:s
```

여기서:

* `gclid`은(는) [!DNL Google Click ID]&#x200B;(GCLID)입니다.
* `s`은(는) 네트워크 유형입니다(검색의 경우 &quot;s&quot;).

#### [!DNL Microsoft Advertising]개 검색 광고

```
{msclkid}:G:s
```

여기서:

* `msclkid`은(는) [!DNL Microsoft Click ID]&#x200B;(MSCLKID)입니다.
* `s`은(는) 네트워크 유형입니다(검색의 경우 &quot;s&quot;).

#### 다른 검색 엔진에 광고 및 검색 광고 표시

```
<Adobe Advertising visitor ID>:<timestamp>:<channel type>
```

여기서:

* &lt;*Adobe Advertising 방문자 ID*>은(는) 방문자별 고유 ID입니다(예: UhKVaAAABCkJ0mDt). *서퍼 ID*&#x200B;이라고도 합니다.

* &lt;*timestamp*>는 YYYYMMMDDHHMMSS 형식의 시간입니다(예: 2019년, 08월, 21일, 19:25:33일의 20190821192533).

* &lt;*채널 유형*>은(는) 클릭 또는 노출을 담당하는 채널 유형입니다.

   * DSP 디스플레이 광고 클릭용 `d`(디스플레이 클릭스루)
   * DSP 디스플레이 광고(디스플레이 뷰스루)의 노출에 대한 `i`
   * `s`(검색 광고 클릭(검색 클릭스루)).

예 `EF ID: WcmibgAAAHJK1RyY:1551968087687:d`
