# PooCodeView
图形验证码，本地校验图形验证码，🌄 随机验证码图文校验，图文校验,提升安全性频繁登录等;





## Usage

```
#import "PooCodeView.h"
@property (nonatomic, strong) PooCodeView *pooCodeView;
```
```
//1.默认
    _pooCodeView = [[PooCodeView alloc] initWithFrame:CGRectMake(10, 100, 120, 50) andChangeArray:nil];
    [self.view addSubview:_pooCodeView];
```

```
//2.自定义
    NSArray *randomArr = @[@"H",@"j",@"q",@"0",@"1",@"2",@"3",@"4",@"5",@"6",@"7",@"8",@"9"];
    _pooCodeView = [[PooCodeView alloc] initWithFrame:CGRectMake(140, 100, 120, 50) andChangeArray:randomArr];
    
    //注意:文字高度不能大于poocodeview高度,否则crash
    _pooCodeView.textSize = 25;
    
    //不设置为blackColor
    _pooCodeView.textColor = [UIColor redColor];
    
    [self.view addSubview:_pooCodeView];
```



## License

This code is distributed under the terms and conditions of the [MIT license](LICENSE).# [randomCode](https://kunnan.blog.csdn.net/)
