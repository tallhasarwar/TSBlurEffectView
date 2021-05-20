# TSBlurEffectView
Add blur effect in iOS with custom blur intensity to your uiview, uilabels, uiimages etc etc

<img width="138" alt="Screenshot 2021-05-20 at 19 26 27" src="https://user-images.githubusercontent.com/32789610/118996447-5dd44e00-b9a1-11eb-89ac-5862b6baf8dc.png"> <img width="130" alt="Screenshot 2021-05-20 at 19 26 44" src="https://user-images.githubusercontent.com/32789610/118996467-60cf3e80-b9a1-11eb-923a-c6a69031aa96.png"> <img width="166" alt="Screenshot 2021-05-20 at 19 27 01" src="https://user-images.githubusercontent.com/32789610/118996486-6462c580-b9a1-11eb-9f21-1e3d498c108e.png">

Low to high intensity


# Installation Manually
To use just download and include TSBlurEffectView.swift into your project and write an extension for UILabel as follow

# Ho to use in UILabel
Write an extension for UILabel as follow

```Swift
    extension UILabel {
      func addBlurrEffect() {
          let blurEffectView = TSBlurEffectView() // creating a blur effect view
          blurEffectView.intensity = 1 // setting blur intensity from 0.1 to 10
          self.addSubview(blurEffectView) // adding blur effect view as a subview to your view in which you want to use
      }
    
      func removeBlurEffect() {
          for subview in self.subviews {
              if subview is UIVisualEffectView {
                  subview.removeFromSuperview()
              }
          }
      }
    }
```
For adding yourUILable.addBlurrEffect() for adding blur effect

And yourUILable.removeBlurEffect() for removing the blur effect

# Ho to use in UIView
To use just download and include TSBlurEffectView.swift into your project and write an extension for UILabel as follow
```Swift
    extension UIView {
      func addBlurrEffect() {
          let blurEffectView = TSBlurEffectView() // creating a blur effect view
          blurEffectView.intensity = 1 // setting blur intensity from 0.1 to 10
          self.addSubview(blurEffectView) // adding blur effect view as a subview to your view in which you want to use
      }
    
      func removeBlurEffect() {
          for subview in self.subviews {
              if subview is UIVisualEffectView {
                  subview.removeFromSuperview()
              }
          }
      }
    }
```
For adding yourUIView.addBlurrEffect() for adding blur effect

And yourUIView.removeBlurEffect() for removing the blur effect

# Ho to use in UIImageView
To use just download and include TSBlurEffectView.swift into your project and write an extension for UILabel as follow
```Swift
    extension UIImageView {
      func addBlurrEffect() {
          let blurEffectView = TSBlurEffectView() // creating a blur effect view
          blurEffectView.intensity = 1 // setting blur intensity from 0.1 to 10
          self.addSubview(blurEffectView) // adding blur effect view as a subview to your view in which you want to use
      }
    
      func removeBlurEffect() {
          for subview in self.subviews {
              if subview is UIVisualEffectView {
                  subview.removeFromSuperview()
              }
          }
      }
    }
```
For adding yourUIImageView.addBlurrEffect() for adding blur effect

And yourUIImageView.removeBlurEffect() for removing the blur effect

You can add it to any UIView directly as well.
