
# Swift Examples


## UIView Background Gradient

```swift
import UIKit
import QuartzCore

// create base view
let view: UIView = UIView(frame: CGRectMake(0, 0, 100, 100))

// create gradient layer
let gradient : CAGradientLayer = CAGradientLayer()

// create color array
let arrayColors: AnyObject[] = [
  UIColor.blueColor().CGColor,
  UIColor.redColor().CGColor
]

// set gradient frame bounds to match view bounds
gradient.frame = view.bounds

// set gradient's color array
gradient.colors = arrayColors

// replace base layer with gradient layer
view.layer.insertSublayer(gradient, atIndex: 0)
```

## Create Dictionary from plist

```swift
let path = NSBundle.mainBundle().pathForResource("samplePlist", ofType: "plist")
let dict = NSDictionary(contentsOfFile: path)
```
