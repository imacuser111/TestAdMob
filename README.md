---
title: 'ADMob'
tags: ADMob
disqus: hackmd
---

ADMob
===

## Table of Contents

[TOC]

## 介紹
[https://drive.google.com/file/d/1mj3rKPpvmdMmVxSMc0CUsRfjk-Koj8nO/view?usp=sharing](https://drive.google.com/file/d/1mj3rKPpvmdMmVxSMc0CUsRfjk-Koj8nO/view?usp=sharing)

## Demo
![](http://badgameshow.com/7hong/wp-content/uploads/2021/07/截圖-2021-07-26-下午1.03.03.png)

## 設定AdMob - 新增應用程式
![](http://badgameshow.com/7hong/wp-content/uploads/2021/07/截圖-2021-07-26-下午2.36.42.png)

## XCode - pod
``` swift 
pod 'Google-Mobile-Ads-SDK'
```
## Add the -ObjC linker flag to Other Linker Flags in your project's build settings:
![](http://badgameshow.com/7hong/wp-content/uploads/2021/07/截圖-2021-07-26-下午2.43.54.png)

## Update your Info.plist
#### 更新您的應用程序的 Info.plist 文件以添加兩個keys：
#### 1. 一個 GADApplicationIdentifier Key，包含您的 AdMob 應用 ID（在 AdMob 用戶界面中標識）的字符串值。 
#### 2. 帶有 Google (cstr6suwn9.skadnetwork) SKAdNetworkIdentifier 值的 SKAdNetworkItems Key，並選擇向 Google 提供這些值的其他買家。

#### 這邊要注意：在實際應用中，重要的是使用您的實際 AdMob 應用 ID，而不是下面列出的ID(ca-app-pub-3940256099942544~1458002511)。
#### 不過，如果您只是想在測試的應用程序中試驗 SDK，則可以使用上面顯示的示例應用程序 ID。

<details>
    <summary>Source Code</summary>

``` swift
<key>GADApplicationIdentifier</key>
<string>ca-app-pub-3940256099942544~1458002511</string>
<key>SKAdNetworkItems</key>
  <array>
    <dict>
      <key>SKAdNetworkIdentifier</key>
      <string>cstr6suwn9.skadnetwork</string>
    </dict>
    <dict>
      <key>SKAdNetworkIdentifier</key>
      <string>4fzdc2evr5.skadnetwork</string>
    </dict>
    <dict>
      <key>SKAdNetworkIdentifier</key>
      <string>2fnua5tdw4.skadnetwork</string>
    </dict>
    <dict>
      <key>SKAdNetworkIdentifier</key>
      <string>ydx93a7ass.skadnetwork</string>
    </dict>
    <dict>
      <key>SKAdNetworkIdentifier</key>
      <string>5a6flpkh64.skadnetwork</string>
    </dict>
    <dict>
      <key>SKAdNetworkIdentifier</key>
      <string>p78axxw29g.skadnetwork</string>
    </dict>
    <dict>
      <key>SKAdNetworkIdentifier</key>
      <string>v72qych5uu.skadnetwork</string>
    </dict>
    <dict>
      <key>SKAdNetworkIdentifier</key>
      <string>c6k4g5qg8m.skadnetwork</string>
    </dict>
    <dict>
      <key>SKAdNetworkIdentifier</key>
      <string>s39g8k73mm.skadnetwork</string>
    </dict>
    <dict>
      <key>SKAdNetworkIdentifier</key>
      <string>3qy4746246.skadnetwork</string>
    </dict>
    <dict>
      <key>SKAdNetworkIdentifier</key>
      <string>3sh42y64q3.skadnetwork</string>
    </dict>
    <dict>
      <key>SKAdNetworkIdentifier</key>
      <string>f38h382jlk.skadnetwork</string>
    </dict>
    <dict>
      <key>SKAdNetworkIdentifier</key>
      <string>hs6bdukanm.skadnetwork</string>
    </dict>
    <dict>
      <key>SKAdNetworkIdentifier</key>
      <string>prcb7njmu6.skadnetwork</string>
    </dict>
    <dict>
      <key>SKAdNetworkIdentifier</key>
      <string>v4nxqhlyqp.skadnetwork</string>
    </dict>
    <dict>
      <key>SKAdNetworkIdentifier</key>
      <string>wzmmz9fp6w.skadnetwork</string>
    </dict>
    <dict>
      <key>SKAdNetworkIdentifier</key>
      <string>yclnxrl5pm.skadnetwork</string>
    </dict>
    <dict>
      <key>SKAdNetworkIdentifier</key>
      <string>t38b2kh725.skadnetwork</string>
    </dict>
    <dict>
      <key>SKAdNetworkIdentifier</key>
      <string>7ug5zh24hu.skadnetwork</string>
    </dict>
    <dict>
      <key>SKAdNetworkIdentifier</key>
      <string>9rd848q2bz.skadnetwork</string>
    </dict>
    <dict>
      <key>SKAdNetworkIdentifier</key>
      <string>n6fk4nfna4.skadnetwork</string>
    </dict>
    <dict>
      <key>SKAdNetworkIdentifier</key>
      <string>kbd757ywx3.skadnetwork</string>
    </dict>
    <dict>
      <key>SKAdNetworkIdentifier</key>
      <string>9t245vhmpl.skadnetwork</string>
    </dict>
    <dict>
      <key>SKAdNetworkIdentifier</key>
      <string>4468km3ulz.skadnetwork</string>
    </dict>
    <dict>
      <key>SKAdNetworkIdentifier</key>
      <string>2u9pt9hc89.skadnetwork</string>
    </dict>
    <dict>
      <key>SKAdNetworkIdentifier</key>
      <string>8s468mfl3y.skadnetwork</string>
    </dict>
    <dict>
      <key>SKAdNetworkIdentifier</key>
      <string>av6w8kgt66.skadnetwork</string>
    </dict>
    <dict>
      <key>SKAdNetworkIdentifier</key>
      <string>klf5c3l5u5.skadnetwork</string>
    </dict>
    <dict>
      <key>SKAdNetworkIdentifier</key>
      <string>ppxm28t8ap.skadnetwork</string>
    </dict>
    <dict>
      <key>SKAdNetworkIdentifier</key>
      <string>424m5254lk.skadnetwork</string>
    </dict>
    <dict>
      <key>SKAdNetworkIdentifier</key>
      <string>uw77j35x4d.skadnetwork</string>
    </dict>
    <dict>
      <key>SKAdNetworkIdentifier</key>
      <string>578prtvx9j.skadnetwork</string>
    </dict>
    <dict>
      <key>SKAdNetworkIdentifier</key>
      <string>4dzt52r2t5.skadnetwork</string>
    </dict>
    <dict>
      <key>SKAdNetworkIdentifier</key>
      <string>e5fvkxwrpn.skadnetwork</string>
    </dict>
    <dict>
      <key>SKAdNetworkIdentifier</key>
      <string>8c4e2ghe7u.skadnetwork</string>
    </dict>
    <dict>
      <key>SKAdNetworkIdentifier</key>
      <string>zq492l623r.skadnetwork</string>
    </dict>
    <dict>
      <key>SKAdNetworkIdentifier</key>
      <string>3qcr597p9d.skadnetwork</string>
    </dict>
  </array>
```
    
</details>

## 初始化移動廣告 SDK
```swift
import GoogleMobileAds

@UIApplicationMain
class AppDelegate: UIResponder, UIApplicationDelegate {

  func application(_ application: UIApplication,
      didFinishLaunchingWithOptions launchOptions: [UIApplicationLaunchOptionsKey: Any]?) -> Bool {

    GADMobileAds.sharedInstance().start(completionHandler: nil)

    return true
  }
}
```

## 宣告變數
``` swift
var adLoader: GADAdLoader!
let nibView = Bundle.main.loadNibNamed("NativeAdView", owner: nil, options: nil)?.first
```

## Initialize the ad loader

``` swift
// MARK: - GADAdLoader
    private func addAdLoader() {
        GADMobileAds.sharedInstance().requestConfiguration.testDeviceIdentifiers = [ "6ead1bb750bcfa2634aece47f1bdc358" ]
        
        let multipleAdsOptions = GADMultipleAdsAdLoaderOptions()
        multipleAdsOptions.numberOfAds = 5
        
        adLoader = GADAdLoader(adUnitID: "ca-app-pub-1953039198708312/2945809803",
                               rootViewController: self,
                               adTypes: [.native],
                               options: [multipleAdsOptions])
        
        adLoader.delegate = self
        adLoader.load(GADRequest())
    }
```

## 實作GADNativeAdLoaderDelegate

<details>
    <summary>Source Code</summary>

``` swift
extension ContentViewController: GADNativeAdLoaderDelegate {
    func adLoader(_ adLoader: GADAdLoader, didFailToReceiveAdWithError error: Error) {
        
    }
    
    func adLoaderDidFinishLoading(_ adLoader: GADAdLoader) {
        
    }
    
    // MARK: - setting adView Data
    func adLoader(_ adLoader: GADAdLoader, didReceive nativeAd: GADNativeAd) {
        print("Received native ad: \(nativeAd)")
        
        guard let nativeAdView = nibView as? GADNativeAdView else { return }
        
        // Set ourselves as the native ad delegate to be notified of native ad events.
        nativeAd.delegate = self
        
        // Populate the native ad view with the native ad assets.
        // The headline and mediaContent are guaranteed to be present in every native ad.
        (nativeAdView.headlineView as? UILabel)?.text = nativeAd.headline
        nativeAdView.mediaView?.mediaContent = nativeAd.mediaContent
//        nativeAdView.mediaView?.contentMode = .scaleAspectFit
        
        // This app uses a fixed width for the GADMediaView and changes its height to match the aspect
        // ratio of the media it displays.
        if let mediaView = nativeAdView.mediaView, nativeAd.mediaContent.aspectRatio > 0 {
            let heightConstraint = NSLayoutConstraint(
                item: mediaView,
                attribute: .height,
                relatedBy: .equal,
                toItem: mediaView,
                attribute: .width,
                multiplier: CGFloat(1 / nativeAd.mediaContent.aspectRatio),
                constant: 0)
            heightConstraint.isActive = true
        }
        
        // These assets are not guaranteed to be present. Check that they are before
        // showing or hiding them.
        (nativeAdView.bodyView as? UILabel)?.text = nativeAd.body
        nativeAdView.bodyView?.isHidden = nativeAd.body == nil
        
        (nativeAdView.callToActionView as? UIButton)?.setTitle(nativeAd.callToAction, for: .normal)
        nativeAdView.callToActionView?.isHidden = nativeAd.callToAction == nil
        
        (nativeAdView.iconView as? UIImageView)?.image = nativeAd.icon?.image
        nativeAdView.iconView?.isHidden = nativeAd.icon == nil
        
        (nativeAdView.starRatingView as? UIImageView)?.image = imageOfStars(from: nativeAd.starRating)
        nativeAdView.starRatingView?.isHidden = nativeAd.starRating == nil
        
        (nativeAdView.storeView as? UILabel)?.text = nativeAd.store
        nativeAdView.storeView?.isHidden = nativeAd.store == nil
        
        (nativeAdView.priceView as? UILabel)?.text = nativeAd.price
        nativeAdView.priceView?.isHidden = nativeAd.price == nil
        
        (nativeAdView.advertiserView as? UILabel)?.text = nativeAd.advertiser
        nativeAdView.advertiserView?.isHidden = nativeAd.advertiser == nil
        
        // In order for the SDK to process touch events properly, user interaction should be disabled.
        nativeAdView.callToActionView?.isUserInteractionEnabled = false
        
        // Associate the native ad view with the native ad object. This is
        // required to make the ad clickable.
        // Note: this should always be done after populating the ad views.
        
        nativeAdView.nativeAd = nativeAd
    }
    
    /// Returns a `UIImage` representing the number of stars from the given star rating; returns `nil`
    /// if the star rating is less than 3.5 stars.
    func imageOfStars(from starRating: NSDecimalNumber?) -> UIImage? {
        guard let rating = starRating?.doubleValue else {
            return nil
        }
        if rating >= 5 {
            return UIImage(named: "stars_5")
        } else if rating >= 4.5 {
            return UIImage(named: "stars_4_5")
        } else if rating >= 4 {
            return UIImage(named: "stars_4")
        } else if rating >= 3.5 {
            return UIImage(named: "stars_3_5")
        } else {
            return nil
        }
    }
    
    func setAdView(view: UIView, _ adView: UIView) {
        // Remove the previous ad view.
        adView.translatesAutoresizingMaskIntoConstraints = false
        view.addSubview(adView)
        
        // Layout constraints for positioning the native ad view to stretch the entire width and height
        // of the nativeAdPlaceholder.
        let viewDictionary = ["_nativeAdView": adView]
        view.addConstraints(
            NSLayoutConstraint.constraints(
                withVisualFormat: "H:|[_nativeAdView]|",
                options: NSLayoutConstraint.FormatOptions(rawValue: 0), metrics: nil, views: viewDictionary)
        )
        view.addConstraints(
            NSLayoutConstraint.constraints(
                withVisualFormat: "V:|[_nativeAdView]|",
                options: NSLayoutConstraint.FormatOptions(rawValue: 0), metrics: nil, views: viewDictionary)
        )
    }
}
```
    
</details>
    
## 設定adView
``` swift
if let adView = self.nibView as? UIView {
	setAdView(view: self.view, adView)
}
```

## 自家廣告設定
### 創建活動廣告
![](http://badgameshow.com/7hong/wp-content/uploads/2021/07/截圖-2021-07-26-下午4.25.22.png)

### 設定曝光比例100%
![](http://badgameshow.com/7hong/wp-content/uploads/2021/07/截圖-2021-07-26-下午4.28.05.png)

## GitHub
[gitHub](https://github.com/imacuser111/TestAdMob)

## 參考資料

[https://developers.google.com/admob/ios/quick-start](https://developers.google.com/admob/ios/quick-start)

[https://stackoverflow.com/questions/60888855/using-admob-for-own-ads-in-house-in-own-application-how](https://stackoverflow.com/questions/60888855/using-admob-for-own-ads-in-house-in-own-application-how)
