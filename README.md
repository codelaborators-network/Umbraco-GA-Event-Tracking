# Google Analytics Events for Umbraco
![Google Analytics Events for Umbraco Logo](https://github.com/codelaborators-network/Google-Analytics-Events-for-Umbraco/blob/master/Logos/logo_200_200.jpg?raw=true "Google Analytics Events for Umbraco Logo")

A package for adding manageable GA Event Tracking to your Umbraco site.

## Install

1. Install the Google Analytics Events for Umbraco package
2. Add the Following code to your master template (order is important)

```javascript

@using UmbracoGAEventTracking;

@Html.IncludeGoogleAnalytics() // Only needed if you have not already included Google Analytics. You can add your GA Key in Umbraco.
@Html.IncludeGaEventTracking()

```

If you would like to use caching to save calls to the database, add this appSetting to your web.config file.

```javascript

<add key="GAEventTracking_CachingTimeInMinutes" value="10"/>

```
### Please read the [Documentation Website](https://codelaborators-network.github.io/Google-Analytics-Events-for-Umbraco/) for more in depth guidelines

