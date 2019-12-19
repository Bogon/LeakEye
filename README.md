# LeakEye

[![Swift 4.0+](https://img.shields.io/badge/Swift-4.0%2B-orange.svg)](https://github.com/zixun/AssistiveButton)

[![Version](https://img.shields.io/cocoapods/v/LeakEye.svg?style=flat)](http://cocoapods.org/pods/LeakEye)
[![License](https://img.shields.io/cocoapods/l/LeakEye.svg?style=flat)](http://cocoapods.org/pods/LeakEye)
[![Platform](https://img.shields.io/cocoapods/p/LeakEye.svg?style=flat)](http://cocoapods.org/pods/LeakEye)
[![Carthage compatible](https://img.shields.io/badge/Carthage-Compatible-brightgreen.svg?style=flat)](https://github.com/Carthage/Carthage) 

LeakEye is a memory leak monitor inspired by PLeakSniffer.

## Family
This library is derived from the [GodEye](https://github.com/Bogon/GodEye) project which can automaticly display Log,Crash,Network,ANR,Leak,CPU,RAM,FPS,NetFlow,Folder and etc with one line of code. Just like god opened his eyes

## Book & Principle

**I has wrote a book named [《iOS监控编程》](),each chapter records the course function of the implementation details and the way to explore.sorry for english friends,this book wrote by chineses.**


## Example

To run the example project, clone the repo, and run `pod install` from the Example directory first.


## Installation

### CocoaPods
LeakEye is available through [CocoaPods](http://cocoapods.org). To install
it, simply add the following line to your Podfile:

```ruby
pod 'LeakEye'
```

### Carthage
Or, if you’re using [Carthage](https://github.com/Carthage/Carthage), add SwViewCapture to your Cartfile:

``` 
github 'Bogon/LeakEye'
```

## Usage
Import the lib:

```swift
import LeakEye
```

Declare an instance variable：

```swift
var eye = LeakEye()
```

Start monitor:

```swift
self.eye.delegate = self
self.eye.start()
```

Implement the delegate:

```swift
func leakEye(leakEye:LeakEye,didCatchLeak object:NSObject) {
    print(object)
}
```

that's all!(就酱)

## Thanks
Thanks for [PLeakSniffer](https://github.com/music4kid/PLeakSniffer),LeakEye is inspired by it.


## 维护者

name: Bogon

email: zhangqixcu@gmail.com

github: [Bogon](https://github.com/Bogon)

## Author

name: 陈奕龙

twitter: [@zixun_](https://twitter.com/zixun_)

email: chenyl.exe@gmail.com

github: [zixun](https://github.com/zixun)

blog: [子循(SubCycle)](http://zixun.github.io/)

## License

LeakEye is available under the MIT license. See the LICENSE file for more info.
