# MultipleLayerArcMenu
MultipleLayerArc Menu is to animate multiple buttons and place them in prefered circular, semi circular or quarter circular format. This menu buttons can be emerged from any corner of the screen with the modified angle. As per the git code, it is expanding from right bottom corner of the screen. Number of buttons in each layer is based on the array of dictionaries passed from a viewcontroller.
# ScreenShot
![simulator screen shot - iphone 6 - 2018-01-31 at 16 12 46](https://user-images.githubusercontent.com/16645242/35618698-bc54ccfe-06a1-11e8-943c-fff00d3b7426.png)

![simulator screen shot - iphone 6 - 2018-01-31 at 15 56 25](https://user-images.githubusercontent.com/16645242/35618718-c8829f7e-06a1-11e8-96db-17db0b5ab56c.png)
# Compatability
Version - Swift 3+, iOS 9+
# Example
```
self._circularMenuVC = MultipleLayerArcMenu.init(listOfButtonDetails: arrayOfMenuButtons, viewController: self, centerButtonFrame: self.optionButton.frame, circularButton: self.optionButton, startAngle: 95, totalAngle: 95, radius: -80)
self._circularMenuVC?._delegateSemiCircularMenu = self
self._circularMenuVC?.showMenuOption()
```

# CallBacks
```ruby
SemiCircularMenuDelegate

---Delegate Method---

func SemiCircularMenuClickedButtonAtIndex(buttonIndex: Int, buttonOutlet: UIButton)
```

# Manual
1. Add MultipleLayerArcMenu.swift to your project
2. Import the same in preferable viewcontroller and initialize as per example (above)
