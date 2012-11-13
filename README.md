LBBlurredImage
============

LBBlurredImage is an UIImageView category that permit to set an image and make this blurred.

Here are an example of what you can achieve:
![](https://raw.github.com/lukabernardi/LBBlurredImage/master/Resources/SimulatorScreenshot.png)

Installation & Use
============

### Installation
- Just grab the two file named `UIImageView+LBBlurredImage.h` & `UIImageView+LBBlurredImage.m` in the Additions group into your project and link with CoreImage.framework .
- `#import "UIImageView+LBBlurredImage.h"` where you need it.

### Use

``` objective-c
[self.imageView setImageToBlur:[UIImage imageNamed:@"example"]
                    blurRadius:kLBBlurredImageDefaultBlurRadius
               completionBlock:^(NSError *error){
                   NSLog(@"The blurred image has been setted");
               }];
```