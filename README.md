# RangeSlider


**[NOTICE from @fullc0de]**  
The original repo seems to be abondoned. However, I will maintain my forked repo later on because it is still used in my project. 


## Summary
A simple range slider made in Swift.

## Screenshot
![](https://github.com/warchimede/RangeSlider/blob/master/Screenshot.png?raw=true)

## Use
This control is **IBDesignable** and uses the **target-action** pattern for change notifications.

In order to be notified when either thumb value changes, register for **.ValueChanged**:

    let rangeSlider = RangeSlider(frame: frame)
    view.addSubView(rangeSlider)
    rangeSlider.addTarget(self, action: "rangeSliderValueChanged:",
                             forControlEvents: .ValueChanged)

## Configuration
The range slider can be customized and information can be accessed through these properties :

  + `minimumValue` : The minimum possible value of the range
  + `maximumValue` : The maximum possible value of the range
  + `lowerValue` : The value corresponding to the left thumb current position
  + `upperValue` : The value corresponding to the right thumb current position
  + `trackTintColor` : The track color
  + `trackHighlightTintColor` : The color of the section of the track located between the two thumbs
  + `thumbTintColor`: The thumb color
  + `thumbBorderColor`: The thumb border color
  + `thumbBorderWidth`: The width of the thumb border
  + `curvaceousness` : From 0.0 for square thumbs to 1.0 for circle thumbs

## License
RangeSlider is available under the MIT License

If you use it and like it, let me know: [@warchimede](http://twitter.com/warchimede)
