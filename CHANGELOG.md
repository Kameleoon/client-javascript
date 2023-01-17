# Changelog
All notable changes to this project will be documented in this file.

## 2.1.0 - 2023-01-17
* Added client initialization with `configDataFile`, which prevents api data call by using custom configuration passed as `configDataFile`.

## 2.0.1 - 2023-01-13
* Bug fix: localStorage data is not saved correctly.

## 2.0.0 - 2022-12-30
* Added support for the new feature flag rules.
* `activateFeature` & `obtainFeatureVariable` are deprecated.
* Renaming of methods: 
  - `obtainVisitorCode` -> [`getVisitorCode`](https://developers.kameleoon.com/javascript-sdk.html#getVisitorCode)
  - `obtainVariationAssociatedData` -> [`getVariationAssociatedData`](https://developers.kameleoon.com/javascript-sdk.html#getVariationAssociatedData)
* Methods added for obtaining experiment and feature flag lists along with feature variables:
  - [`getExperimentList`](https://developers.kameleoon.com/javascript-sdk.html#getExperimentList)
  - [`getExperimentListForVisitorCode`](https://developers.kameleoon.com/javascript-sdk.html#getExperimentListForVisitorCode)
  - [`getFeatureList`](https://developers.kameleoon.com/javascript-sdk.html#getFeatureList)
  - [`getFeatureListForVisitorCode`](https://developers.kameleoon.com/javascript-sdk.html#getFeatureListForVisitorCode)
  - [`getFeatureAllVariables`](https://developers.kameleoon.com/javascript-sdk.html#getFeatureAllVariables)
* Added support of `is among the values` operator for Custom Data

## 1.0.9 - 2022-08-03
* Added update campaigns and feature flag configurations instantaneously with Real-Time Streaming Architecture: [`documentation`](https://developers.kameleoon.com/javascript-sdk.html#streaming) or [`product updates`](https://www.kameleoon.com/en/blog/real-time-streaming)
* Added a new method [`onUpdateConfiguration`](https://developers.kameleoon.com/javascript-sdk.html#onUpdateConfiguration) to handle events when configuration data is updated in real time.
* Added support for **Experiment** & **Exclusive Campaign** conditions. Related to [`triggerExperiment`](https://developers.kameleoon.com/nodejs-sdk.html#triggerexperiment)
* Fixed an issue when an user which was already registered with a variation gets new randomly selected variation. Related to [`triggerExperiment`](https://developers.kameleoon.com/javascript-sdk.html#triggerexperiment)
* Added KameleoonData [`Device`](https://developers.kameleoon.com/javscript-sdk.html#device) data. Possible values are: **PHONE**, **TABLET**, **DESKTOP**. 
* Removed KameleoonData `Interest`
* Added support of `is among the values` operator for Custom Data

## 1.0.8 - 2022-06-14
* Fixed an issue when tracking data could be sent twice. Related to: [`triggerExperiment`](https://developers.kameleoon.com/javascript-sdk.html#triggerexperiment) & [`activateFeature`](https://developers.kameleoon.com/javascript-sdk.html#activatefeature)

## 1.0.7 - 2022-04-12
* Added method for retrieving data from remote source: [`retrieveDataFromRemoteSource`](https://developers.kameleoon.com/javascript-sdk.html#retrievedatafromremotesource)

## 1.0.6 - 2022-02-10
* Added support of multi-environment for feature flags, Related to [`activateFeature`](https://developers.kameleoon.com/javascript-sdk.html#activatefeature), [`obtainFeatureVariable`](https://developers.kameleoon.com/javascript-sdk.html#obtainfeaturevariable)
* Added checking for status of site_code (Enable / Disable). Related to [`activateFeature`](https://developers.kameleoon.com/javascript-sdk.html#activatefeature) and [`triggerExperiment`](https://developers.kameleoon.com/javascript-sdk.html#triggerexperiment)
* Fixed issue with overlapping periods for scheduling. Related to [`activateFeature`](https://developers.kameleoon.com/javascript-sdk.html#activatefeature)

## 1.0.5 - 2021-11-03
* Fixing add data limitation

## 1.0.4 - 2021-10-28
* Add schedules feature flag

## 1.0.2 - 2021-10-06
* Fixed types for Browser, Conversion, Interest, PageView
