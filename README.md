# WebPageLoader

A piece of simple code for taking snapshot of web pages for Cocoa, written in Swift 2.0 syntax.

## Install

Just drag the two files into your project.

## Usage

```swift
let loader = WebPageLoader(snapshotSize: yourImageView.bounds.size)

let request = ...

loader.loadRequest(request) { (detail, initialRequest) in
  if let detail = detail {
    yourImageView.image = detail.snapshot
  }
}
```

## License

This project is released under Apache 2.0 License. See the LICENSE file.
