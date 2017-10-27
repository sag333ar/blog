---
layout: post
title:  "Swift dial phone number"
date:   2017-02-07 11:00:00
categories: Swift
tags: IBAction dial phone canOpenURL openURL
---

Following is a code snippet for dialing phone number through code in iOS Swift

```swift
@IBAction func btnDialPhone(_ sender: AnyObject) {
     if let url = URL(string: "tel://123456789"), UIApplication.shared.canOpenURL(url) {
               UIApplication.shared.openURL(url)
     }
}
```