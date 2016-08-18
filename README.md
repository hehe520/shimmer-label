# shimmer-label
闪光字体，支持多种闪光模式，用法简单，shimmer label shimmering

话不多说，直接看代码吧，和 facebook 的效果一样，一行代码就能开启闪烁，可以自定义多种样式

CKShimmerLabel 就是我的 label 类，创建它，用 startShimmer 方法就可以开启闪烁了
```
    self.label1 = [[CKShimmerLabel alloc] init];
    self.label1.frame = CGRectMake(20, 35, 200, 35);
    self.label1.text = @"hello world 1";
    self.label1.textColor = [UIColor grayColor];
    self.label1.font = [UIFont systemFontOfSize:30];
    [self.label1 startShimmer];                 // 开启闪烁
    [self.view addSubview:self.label1];
```

一些可以修改的属性

```
ShimmerType shimmerType;          // 闪烁类型，默认LeftToRight
BOOL repeat;                      // 循环播放，默认是
CGFloat shimmerWidth;             // 闪烁宽度，默认20
CGFloat shimmerRadius;            // 闪烁半径，默认20
UIColor *shimmerColor;            // 闪烁颜色，默认白
NSTimeInterval durationTime;      // 持续时间，默认2秒

直接 self.label1.shimmerColor = [UIColor yellowColor]; 就可以修改颜色
```

快下载看看效果吧



