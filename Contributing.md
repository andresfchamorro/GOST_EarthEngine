### Added by Yingxu Song.
- File: TimeSeries_Vegetation\Modis.js
- Change the AOI, I have no access to your personal file, or you could make it public.
  
From:
```
var AOIs = ee.FeatureCollection('users/afche18/Ethiopia_AOI');
```
To:
```
var AOIs = ee.FeatureCollection('USDOS/LSIB_SIMPLE/2017')
  .filter(ee.Filter.eq('country_na', 'Ethiopia'));
```