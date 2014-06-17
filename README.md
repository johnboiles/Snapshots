# Snapshots for Xcode

### An Xcode Plugin to show the state of FBSnapshot Tests.

I think Facebook have [view testing](https://github.com/facebook/ios-snapshot-test-case) right. I don't think Xcode's quite there yet, so I built a plugin to fix this. 

![Screenshot](https://raw.githubusercontent.com/orta/Snapshots/master/web/screenshot.jpg)

#### Features

* Showing new images as they're created
* Showing the differences between failed snapshot tests
* Open specific or all diffs in Xcode

#### Installation

Go look on Alcatraz for "Snapshots", or clone this repo and hit build then restart Xcode. Alcatraz is better, you get updates with no effort.

#### Contributing

It's actually _way_ easier to work on Plugins than you think. Hitting run in Xcode on this project will open a new Xcode with a working lldb instance and you can work on it like any other app. Contributions are extremely welcome of course, large visual design changes should probably be talked about in an issue first FWIW.

#### Unknowns

Currently this only works if you're using XCTests or Expecta. Kiwi has it's own test runner, and I've been focusing on what I use personally. 

If you're using Expecta I really recommend my buddy dB's extension for Expecta: [EXPMatchers+FBSnapshotTest](https://github.com/dblock/ios-snapshot-test-case-expecta). It automates the whole setup process + adds nice language around tests.