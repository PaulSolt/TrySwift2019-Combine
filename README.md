# TrySwift2019-Combine
Materials for TrySwift 2019 Combine Workshop

Bookmark this link and check again for any additional instructions.

## Mac Prep (Downloads)

1. Download and install Xcode 11 Beta 7 from [Beta Software Downloads](https://developer.apple.com/download/)
2. Optional: You can install Catalina on an external SSD
      1. NOTE: You don't need to install Catalina, the new Xcode 11 Simulators are fast enough for rapid prototyping.
      3. Xcode 11 works on both Mojave and Catalina, so I'll include my current setup beta macOS setup below.

## Recommended Videos

Watching these videos will help you undestand the terminology and concepts so that you can dive right in.

* Watch [WWDC 2019: Introducing SwiftUI: Building Your First App](https://developer.apple.com/videos/play/wwdc2019/204/) to dive into SwiftUI
* Watch [WWDC 2019: SwiftUI Essentials](https://developer.apple.com/videos/play/wwdc2019/216/) to learn what's possible
* Watch [Data Flow Through SwiftUI](https://developer.apple.com/videos/play/wwdc2019/226/)
* Watch [Introducing Combine](https://developer.apple.com/videos/play/wwdc2019/722/)
* Watch [Combine in Practice](https://developer.apple.com/videos/play/wwdc2019/721/)

## Resources (Lower priority)

It may take 2-3 hours to skim content in the release notes. Skimming the topics and skipping sections is best, focus on anything relating to Combine, SwiftUI, Swift, and issues/workarounds.

* Read the [release notes for Xcode 11](https://developer.apple.com/documentation/xcode_release_notes/xcode_11_beta_7_release_notes)
* Read the [release notes for iOS 13](https://developer.apple.com/documentation/ios_ipados_release_notes/ios_ipados_13_beta_8_release_notes)

## (Optional) Catalina Install on External SSD

I am running Catalina Beta 10.5 beta 7 on an external SSD with my MacBook Pro 2018 (Samsung T5 500GB ~$100). 

Formatting it was a bit tricky — my Rough notes are to:

1. Open Disk Utility 
1. Show all devices 
2. GUID Partition
3. AFS Format

After install you should be able to hold `Option` on boot to choose the startup disk. Just shutdown completely before removing your SSD drive. 

Updates: Once you install, it's easy to update to the latest beta by using the normal Software Update from System Preferences.

## SwiftUI and Combine Practical Notes

1. Error messages are currently very misleading. If you see a number literal can't be converted to CGFloat, most likely you have a syntax error somewhere 10 lines above/below false error.
2. Xcode will crash a lot, so you'll need to close/reopen a lot.
3. Indentation is buggy, but sometimes fixes itself as you type the placeholders or `:`
4. Release notes can help you with some of the current issues.
5. There are issues with Text("Long .... values") clipping when using `nil` for `lineLimit`, just use `Int.max` for now.

      Text("my long line of text ... that keeps on going")
        .lineLimit(Int.max)

... more notes to come
