---
title: "Non-standard `DataTransfer` APIs have been deprecated"
date: "2018-09-06T05:19:00-04:00"
categories: ["dom"]
tags: []
versions: ["63"]
references:
    - url: "https://bugzilla.mozilla.org/show_bug.cgi?id=1453153"
      title: "Bug 1453153 - Add a pref to disable the DataTransfer moz*At APIs for content"
---
The non-standard `mozGetDataAt`, `mozSetDataAt`, `mozClearDataAt` and `mozTypesAt` methods on the [`DataTransfer`](https://developer.mozilla.org/docs/Web/API/DataTransfer) interface, along with the `mozItemCount` property, are now considered deprecated and disabled on the Nightly channel as of Firefox 63. Given that Telemetry proves no public usage, these APIs will be completely removed in the near future.

Use the standard alternatives instead, including the `getData`, `setData` and `clearData` methods as well as the `items` property.
