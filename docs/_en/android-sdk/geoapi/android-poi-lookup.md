---
title: POI Lookup
tag: [guide, android, geo, poi-lookup]
ref: 3-sdk-android-geo-poi-lookup
---

POI Lookup API provides basic information of POI(scenic spot, tide stations, currents stations, etc.)

| Interface code| Interface  | Class |
| ----------- | --------------- | ---------- |
| geoPoiLookup| POI lookup  | GeoPoiResponse |

## Parameters

**GeoPoiLookupParameter**

{% include params.html p="location-geo geo-type city number lang-def" %}

## Sample code

```java
public void geoPoiLookup(GeoPoiLookupParameter parameter, Callback<GeoPoiResponse> callback);
```

## Response

**GeoPoiResponse**

{% include api-response.html group="geo_poi" type="poi" prefix="poi" update=0 fxlink=0 %}
<!-- 
| Property | Description | Example |
| ---------- | -------- | --------------- |
| getCode | See [Status Code](/en/docs/resource/status-code/) | 200 |
| getPoi | City data | List&lt;Location&gt; |


**Refer**

| Property | Description  |  Type |  Example  |
| ---------- | ----------- | ------------------ | ------------ |
| getSources | Data source and other statements  | List&lt;String&gt; | QWeather     |
| getLicense | Data license     | List&lt;String&gt; | QWeather Developers License |


**Location**

| Property | Description | Example |
| ------------ | ----------------------- | --------- |
| getName | POI name | Beijing Zoo |
| getId | Location ID | 10101020006A |
| getLon | Longitude of the POI | 116.33000 |
| getLat | Latitude of the POI | 39.93000 |
| getAdm2 | Name of the superior administrative division of the POI | Beijing |
| getAdm1 | The first-level administrative region to which the POI belongs | Beijing |
| getCountry | Country name of the POI | China |
| getTz | [Timezone](/en/docs/resource/glossary/#timezone) of the POI | Asia/Shanghai |
| getUtcOffset | The number of hours offset between local time and UTC time, refer to [UTC-Offset](/en/docs/resource/glossary/#utc-offset) | +08:00 |
| getIsDst | Is the location currently observing Daylight Saving time<br />`1` in daylight saving time <br /> `0` not in daylight saving time | 0 |
| getType | POI type | scenic |
| getRank | [Location Rank](/en/docs/resource/glossary/#rank) | 10 |
| getFxLink | Responsive web page of this location, easy to embed in your website or APP | https://www.qweather.com | -->
