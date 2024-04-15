![IAB Tech Lab](https://drive.google.com/uc?id=10yoBoG5uRETSXRrnJPUDuONujvADrSG1)

# OpenRTB Advisory для Open Measurement SDK 

**Рабочий черновик** | Июль 2018

### Область применения

Этот документ рекомендует реализаторам OpenRTB на стороне покупателей (DSP, покупатели), как читать сигналы от продавцов, указывающие на наличие нового инструмента просмотра IAB Tech Lab, Open Measurement SDK. Этот документ дополняет руководство, приведенное в [Open Measurement SDK Onboarding Guide for Integration Partners](https://s3-us-west-2.amazonaws.com/omsdk-files/docs/IAB+Open+Measurement+SDK+Onboarding_GA+version.pdf).

OpenRTB 3.0 и AdCOM 1.0 находятся в бета-версии с 24 июля по 24 сентября 2018 года, что позволяет оставлять публичные комментарии и проводить бета-тестирование. Руководство по внедрению OMSDK выпущено вместе с бета-версией OpenRTB 3.0 и AdCOM 1.0.

### О OpenRTB

Проект RTB, ранее известный как консорциум OpenRTB, собрался в ноябре 2010 года для разработки спецификации API для компаний, заинтересованных в открытом протоколе для автоматизированной торговли цифровыми медиа на широком спектре платформ, устройств и рекламных решений.

OpenRTB 2.5 - это последняя версия для публичного принятия, а OpenRTB 3.0 прошла общественную экспертизу, которая будет завершена позднее в 2018 году.

OpenRTB версий 2.1-2.5 можно найти по адресу [https://iabtechlab.com/openrtb](https://iabtechlab.com/openrtb) 

Дополнительная информация о спецификациях OpenRTB и рабочей группе OpenRTB: [https://iabtechlab.com/openrtb](https://iabtechlab.com/openrtb) 

### О Open Measurement SDK

Комплект разработки программного обеспечения Open Measurement (OM SDK) предназначен для облегчения сторонних измерений просматриваемости и верификации рекламы, подаваемой в мобильные приложения, без необходимости использования нескольких комплектов разработки программного обеспечения (SDK) поставщиков услуг верификации рекламы (поставщиков измерений). OM SDK разрабатывается и управляется рабочей группой Open Measurement Working Group (OMWG).

Дополнительные сведения о OMSDK и OMWG: [https://iabtechlab.com/omsdk](https://iabtechlab.com/omsdk) 

### О IAB Tech Lab

Технологическая лаборатория IAB (Tech Lab) - это некоммерческий консорциум по исследованиям и разработкам, который разрабатывает и предоставляет стандарты, программное обеспечение и услуги для стимулирования роста эффективной и устойчивой глобальной экосистемы цифровых медиа. IAB Tech Lab, в состав которой входят цифровые издатели и компании, занимающиеся рекламными технологиями, а также маркетологи, агентства и другие компании, заинтересованные в интерактивном маркетинге, стремится обеспечить рост брендов и СМИ за счет прозрачной, безопасной и эффективной цепочки поставок, более простых и последовательных измерений и лучшего рекламного опыта для потребителей, уделяя особое внимание развитию мобильных и ТВ/цифровых видеоканалов. В портфолио IAB Tech Lab входит служба стандартизированной идентификации DigiTrust, работающая в режиме реального времени и предназначенная для улучшения цифрового опыта потребителей, издателей, рекламодателей и сторонних платформ. В состав совета директоров входят AppNexus, ExtremeReach, Google, GroupM, Hearst Digital Media, Integral Ad Science, Index Exchange, LinkedIn, MediaMath, Microsoft, Moat, Pandora, PubMatic, Quantcast, Telaria, The Trade Desk и Yahoo! Japan. Основанная в 2014 году, IAB Tech Lab имеет штаб-квартиру в Нью-Йорке, офис в Сан-Франциско и представительства в Сиэтле и Лондоне.

Узнать больше о лаборатории IAB Tech Lab можно здесь: https://www.iabtechlab.com/

### Лицензия

Лицензия OpenRTB Specification the IAB Tech Lab распространяется на условиях Creative Commons Attribution 3.0 License.   Чтобы просмотреть копию этой лицензии, посетите[ creativecommons.org/licenses/by/3.0/](http://creativecommons.org/licenses/by/3.0/) или написать по адресу Creative Commons, 171 Second Street, Suite 300, San Francisco, CA 94105, USA.



# OM SDK support in OpenRTB Version 2.0 to 2.5

OpenRTB 2.0 - 2.5 может быть легко расширен для поддержки OMSDK путем взаимодействия:

1. Если OMID доступен для данного оттиска в заявке на участие в торгах

2. Если объявление, используемое в тендерном ответе, требует OMID

3. "Имя партнера", присваиваемое Издателям, установившим OMSDK

Чтобы поддержать это, список API Frameworks в OpenRTB должен быть расширен значением для OMID. Расширьте список 5.6 API Frameworks следующим образом:

## List 5.6 API Frameworks

<table>
  <tr>
    <td>Значение</td>
    <td>Описание </td>
  </tr>
  <tr>
    <td>1</td>
    <td>VPAID 1.0</td>
  </tr>
  <tr>
    <td>2</td>
    <td>VPAID 2.0</td>
  </tr>
  <tr>
    <td>3</td>
    <td>MRAID-1</td>
  </tr>
  <tr>
    <td>4</td>
    <td>ORMMA</td>
  </tr>
  <tr>
    <td>5</td>
    <td>MRAID-2</td>
  </tr>
  <tr>
    <td>6</td>
    <td>MRAID-3</td>
  </tr>
  <tr>
    <td>7</td>
    <td>OMID-1</td>
  </tr>
</table>


В OpenRTB 2.0 и 2.1 значение 6 отсутствует. При расширении существующей реализации OpenRTB 2.0 или 2.1 рекомендуется пропустить значение 6 и использовать 7 для указания поддержки OMID, чтобы сохранить возможность обновления.

## Bid Request

Поле "api" в **Баннере, видео или нативном объекте** должно использоваться для указания доступности OMID. Это поддерживается в OpenRTB 2.0+.

### Banner/Video/Native/Audio Object

<table>
  <tr>
    <td>Атрибут</td>
    <td>Тип</td>
    <td>Описание</td>
  </tr>
  <tr>
    <td>api</td>
    <td>integer array</td>
    <td>Список поддерживаемых API Frameworks для данного отпечатка. См. список 5.6. Если API не указан в явном виде, предполагается, что он не поддерживается.</td>
  </tr>
</table>


## Bid Response

Поля "apis" и "api" в **Объекте заявки** должны использоваться для указания того, что объявление, используемое в заявке, требует использования OMID. Поле "apis" поддерживается в OpenRTB 2.6, а поле "api" - в OpenRTB 2.4+. Хотя это соответствует принципам дизайна OpenRTB, должна быть возможность модифицировать эти поля в более ранних версиях OpenRTB, поскольку SSP и DSP должны изящно игнорировать поля, которые они не понимают.

### Bid Object

<table>
  <tr>
    <td>Атрибут</td>
    <td>Тип</td>
    <td>Описание</td>
  </tr>
  <tr>
    <td>apis</td>
    <td>integer array</td>
    <td>Список API, требуемых разметкой, если это применимо. См. список 5.6.</td>
  </tr>
  <tr>
    <td>api</td>
    <td>integer</td>
    <td><i>ПРИМЕЧАНИЕ: Утратил силу в пользу целочисленного массива apis в OpenRTB 2.6.</i> API требуется в разметке, если применимо. См. список 5.6.</td>
  </tr>
</table>


# Особые указания для нативной рекламы

OpenRTB Native 1.2 поддерживает OMID с некоторыми дополнительными расширениями через объект 'eventtrackers'.  Он должен использоваться в "Объекте запроса трекеров событий" (раздел 4.7 OpenRTB Dynamic). [Native Ads API Specification Version 1.2](https://www.iab.com/wp-content/uploads/2018/03/OpenRTB-Native-Ads-Specification-Final-1.2.pdf)).

Рекомендуемые значения для "Event Trackers Request Object" следующие:

* **_Событие_** должно быть установлено пользовательское значение "555", чтобы указать, что это OMID, и SSP и издатель будут определять, когда выполнять сценарий OMID.

* **_Метод_** всегда должно быть "2" для JS.  Предыдущее руководство по использованию '555' не является необходимым, если только скрипт не является JS или не-img.

* В стандартное поле eventrackers.url необходимо вставить javascript **_URL_**.

* Трекеры событий OMID могут включать два значения расширения, которые SSP/издатель должен передать OMID при их предоставлении:

    * "vendorKey"

    * "verification_parameters"

<table>
  <tr>
    <td>Объект</td>
    <td>Значение</td>
    <td>Название</td>
  </tr>
  <tr>
    <td>event</td>
    <td>555 </td>
    <td>OMID - new custom value</td>
  </tr>
  <tr>
    <td>methods</td>
    <td>2 </td>
    <td>JS (existing value of 2)</td>
  </tr>
</table>


**Sample bid response**

```
"eventtrackers" { 
  "event": 555  // New, custom value to signify OMID  
  "method": 2  // Previous guidance recommended a value of '555' but '2' is preferred for Javascript  
  "url": "https://verification.com/omid_verification.js"  // This is where DSPs add their actual Javascript URL for measurement  
  "ext": {     // Custom extensions that any exchange can support; these extensions are strongly recommended for SSPs and DSPs to support as part of their OMID support	  
    "vendorKey":  // The vendor key for the company providing the OMID javascript, e.g. "company.com-omid"  
    "verification_parameters":  //Additional verification parameters for the OMSDK, populated by e.g,. "[parameters string]"
	}

}
```


# **OpenRTB and AdCOM**

Заявки на участие в торгах будут включать два новых поля для идентификации партнерской интеграции.  В OpenRTB 2.x и 3.0 эти поля будут представлены в разных объектах, но названия и типы полей в обоих протоколах одинаковы.

<table>
  <tr>
    <td>Атрибут</td>
    <td>Тип</td>
    <td>Описание</td>
  </tr>
  <tr>
    <td>omidpn</td>
    <td>string </td>
    <td>Идентификатор интеграции OM SDK.  Это то же самое, что и параметр "name" объекта OMID Partner.</td>
  </tr>
  <tr>
    <td>omidpv</td>
    <td>string</td>
    <td>Версия интеграции OM SDK.  Это то же самое, что и параметр "versionString" объекта OMID Partner.</td>
  </tr>
</table>


Обратите внимание, что эти поля дополняют массив фреймворков API, который содержится в поле "api" в OpenRTB 2.x и в поле 'apis' в AdCOM.  Массив API-фреймворков должен содержать значение 7, чтобы указать на поддержку OMID 1.0.

### **OpenRTB 2.x**

Эти два поля будут добавлены в объект расширения в заявке.  Существует несколько вариантов использования объекта расширения.  В этом разделе перечислены три варианта.

#### *BidRequest.Source.Ext*

Объект BidRequest.Source описывает источник запроса на участие в торгах OpenRTB 2.x.  Добавление "omidpn" и "omidpv" в Source.Ext будет уместно, если сертификация применяется ко всем размещениям в заявке.

```
"source" {  
  "ext": {  
    "omidpn": "MyIntegrationPartner",  
    "omidpv": "7.1"  
   }  
},  
"imp" [{  
  "banner": {  
    "api": [7]  
  }  
}]  
```


### OpenRTB 3.0 and AdCOM 1.0  (Currently in Beta)

Новая спецификация AdCOM представляет данные рекламного запроса в OpenRTB 3.0.  В отличие от OpenRTB 2.x, поля "omidpn" и "omidpv" будут расширениями в объекте "events", определенном в протоколе (AdCOM 1.0 в настоящее время находится в бета-версии).

#### *Event Trackers*

OMID-возможности запроса на участие в торгах кодируются в объекте "События", что делает его логичным местом для размещения информации о партнере.

```
"events" {
  "apis": [7]  
  "ext": {  
 	 "omidpn": "MyIntegrationPartner",  
 	 "omidpv": "7.1"  
}
```

# OM SDK Guidance

Более подробная информация об Open Measurement SDK, включая [руководство по внедрению](https://s3-us-west-2.amazonaws.com/omsdk-files/docs/IAB+Open+Measurement+SDK+Onboarding_GA+version.pdf), доступна на сайте [https://iabtechlab.com/omsdk](https://iabtechlab.com/omsdk).

## Поддержка 

Если вам нужна поддержка для интеграции OM SDK в ваше приложение или Ad SDK или у вас есть вопросы о том, как использовать OM SDK, пожалуйста, отправьте письмо по адресу omsdksupport@iabtechlab.com. 
