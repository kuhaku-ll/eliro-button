# 猫猫按钮 / Hiiro 按钮 / Hiiro Button

![https://t.bilibili.com/97236535?type=2](https://cdn.jsdelivr.net/gh/blacktunes/hiiro-button@master/public/img/hiiro.png)

### Hiiro...Hiiro...寂しい

 - https://hiiro.club/

### 相关链接：

- [Hiiro 的 Bilibili 直播间](https://live.bilibili.com/21919321)



### 参与完善本项目

- 您可以在[Issues](https://github.com/blacktunes/hiiro-button/issues)提出您的建议。

  - 若是请求添加新语音，请使用指定的**issues模板**
  - 不熟悉**github**的用法也可以到[Bilibili](https://space.bilibili.com/1384118)和我联系

- 如果您可以进行开发，那么请**Fork**本项目进行修改，完成修改后在本项目中发起一个**Pull Request**，详细说明请查看以下条目
  > **Pull Request**请提交至**dev**分支

### 添加或修改音频/完善翻译

音频文件推荐使用**mp3**格式，请先音量标准化，然后放入`public/voices/`目录

所有的分类和音频信息都存储在`setting/translate`目录的`json`文件中，**添加或修改音频信息**、**完善翻译**，你需要修改对应文件中的内容

`locales.json`和`category.json`分别为 UI 界面翻译和分类信息，请不要修改文件名，语音信息可以使用除此外的任意名称，可使用多个`json`文件方便管理语音

可使用`schema`文件夹中的`json`文件增加`json schema`约束和代码提醒

`category.json`结构示例如下：

```jsonc
[
  {
    // 分类命名
    "name": "名言",
    // 是否隐藏
    "hide": true,
    "translate": {
      // 分类中文翻译
      "zh-CN": "猫猫名言~",
      // 分类英文翻译
      "en-US": "witticism~"
    }
  }
]
```

语音文件结构示例如下：

```jsonc
[
  {
    // 语音命名
    "name": "baba",
    // 语音文件名
    "path": "baba.mp3",
    // 是否隐藏
    "hide": true,
    "translate": {
      // 语音中文翻译
      "zh-CN": "米娜我是你爸爸",
      // 语音英语翻译
      "en-US": "I'm your Baba"
    },
    // 语音所属分类(对应category的name)
    "category": "名言",
    // 以下属性为可选
    // hover时显示图片，请放到public/voices/img目录
    "usePicture": {
      "zh-CN": "",
      "en-US": ""
    },
    // 添加时间
    "date": "2020-11-11",
    // 语音出处
    "mark": {
      "title": "【Hiiro】读评论 学中文 DD们的评论都是什么东西啊？",
      "time": "0:01~0:03",
      "url": "https://www.bilibili.com/video/BV1ET4y177A8"
    }
  }
]
```
                                              7.                                                                                  
                                                                                                                                  
                                        .:i;;i.                                                                                   
                                    ..   :;. :r.                            .:::::.;7S                                            
                                  iii,.    , ::                         ,:iii:.   r772                                            
                              7Sr;:,:::i::.;.,           .......   .,iii,.      72;;rX                                            
                              aS;r;,      :i::;ii,,iii;ii::,::i:;Xr:,         rBBiiiX;                                            
                             ,.2i;i2Z;    ..     .:7.                       .X7ZX;r7ri                                            
                            ;. ;riiiZ@a;:                                  ;r     raS.                                            
                         . ,,, ,rXXi,; :i;.          .,:iiirr777;.       .i,        ;i                                            
                            :   S7X . ,  .i:     iZ0BW@MMMMMMMMMMMMM0     . .         i                                           
                         .,     ;          ,   SMMMMMMMMMMMMMMMMMMMMMMW.   . . .   .2WBW@WBB882;                                  
                          ,    i        . .   MMMMMM@0ZS7i:,,.,:ii;7S8MM:   . .     ;MMMMMMMW7MMZ                                 
                      20BWXZW@MMM8     . .  ;MMB2i                                ;; 0MBBWBWaXWM                                  
                     WM@:XBMM@MMM2    . .   ii                           ,X:      7MM0M8BB8S0WMa                                  
                     :MZX8WBBB8@M,;W   .                       .  .     :ZXW   :0S rMaM@WWB022Mi                                  
                      ZM@8S8WWBMB@M8,:     ..         .         .  i.   XS.ar ,200, 8MMB7Z@B00M:                                  
                      iMXaBWB0BM0M2        .   .  .,           ..  :r   rX SBBaZr;rSS8WMB8a8Z@M..                                 
                       MWBBB87BMMW        .       :   .         .   X  iria;7.88arrSXiZ8WZS88iBM;,,                               
                       WW2Z2SW@MMr  .      .   .  r    .         .  i,:8B;rr2aX2ZZX:S22;ZWB00BWMi ii                              
                    i MMSSBZZWarW  .  .   .       S    .      . .   ZZZM.i@0SS7:Z70B22:M@arZBWMX   ;;                             
                   7. .MMW00ZB8W; ..   .  .    :,SZ,.  .     .....  XaX2:ZBB2S.aXZ2r   7M8S00MMW7   7:                            
                  r,   XM@0Z;XM@  :   .   7  ,::,;0   ..... ....... 7 ZiZZ  X7SS     ,  8MM0BMW8MW . X                            
                 ii   ZW@M008MM  :.    . .2:     2B, i,. .,..,.,.  ,i  i,:   :.      .i  ZMM@M@0BMX:7 ;                           
                 7.7 @MWWM@WMM   :    .   27    :i   Xi ..:,.,,..: : ,8M     .        ;   XMMBM     Mr:                           
                iiB: WZXBMMMW   .:     .  SX.   BMaa .i  .,,,,..ia BMMMMM2   :        i.    ZWBM   ,2Zr.                          
                XaM     @MMr    ,.    .   Xr, ZMMMMMM2@8:::i;iX;7iWM@@W72MM.i.  .   , :       2MM  :2;a:                          
                8Z;  ,:MB,      ,. .   ,  .20MMMMWX2BM@WX:ii:i;7 ;i MMMW0MMa;  i,   ;.:, .. i7 2@: i2;XX                          
                B;r  :@MX       X  ;   :,  8MM2 MMZaMMM,           ,M2Z@8SMZ  ;,    W:i7.XZMMZ .Z, i2,7;                          
                B:7 ,r2r .M@@B..2 ;Z    :i  MM  M@0M020B            SXXZrX2:.X,    ri,aZi ,MM  X8X;rZ.                            
                7,X i;Z;  WMM: 7Z.ZB     i7  a7 Z;iSZ:;S            rr:.iai7S     ;0 ZiiX,;Z. ia.a;XS                             
                  7.;aaS  ;Mr X27XrX7     .7r;.  X7:.,;:                   X   . :ZX r    X  ;8. Z72                              
                  7;a; 2..rr      S 8,      ;8;   ,..     ,;:i;;;X        X, .. ,S:7     ;r 7X  ;07                               
                  ,Z2  Z:,S:         2.SX  . 7Z           .277r77S       ,X ., ,S,.X    .X,i    Xi                                
                   7Z  7a,Z:          a207i.  8X.          :7;;i;     ..ia,.,..X,.,7                                              
                        Xa8i          7272:Xr::Z;rii..       . ,;, :;77;S2 ., X: . 7                                              
                         .2X          X    .rX7S8iirrrr;7rX0MMMMMM8X;i:.2; 87i:    i:                                             
                                      07;ii7:.  ,. ::i,r:i27.8MM;.XZ;,;,S.S2rX;X2Za8000,                                          
                                     .0BW08888ZS2a2 ,;SX;Sa,:i,7i:;27:;727W08BW000Ba22,                                           
                                     2   ZWB88BWBWMSii  SX:       .rSi  80W000ZZZ008X;                                            
                                    :: S008ZZZ888ZB@a;:0:            0X XMB808088ZZ8800:                                          
                                    SS002Z808088800@  77             i0  ,@B0080808822a0Zi                                        
                                   2WZ2SaZ08080800B@: 2  8MM8  XMM@   0:.S@088ZZ8Z88B8Z2Z8Z                                       
                                  7BS2a0W0aZZ8Z8Z8B@22@i MMM2;rSMMM.  WX:aW8Z8ZZZZZZZ@B80aZ0                                      
                                 7BSZ08W0ZZaZZZZ8Z8@7   ;S: 72Z2 ., ZB   SM88ZW000000X02SB8ZB                                     
                                :WZBZ;ZZZBZ0080WZ80M@i ,M2  ..   i  .WB,SM@@@BBWr728B8.7  X0W8                                    
                                WBZ:  ;;W08S;r@WBMMWSr:@B   ;S80Z;  .8M  .2aS2WZ;.,.iZii.  ;:i                                    
                                2.  :  8Z;...00X,0a    ,0XrXS28aa7aM8Ma    X ;7;.i:,0: aX:.X.                                     
                               ,r  7B rW .i,X;r X,  .iraaX,,X    :7W0,@   :;aZ X;:i2XrS :X,S.                                     
                               .S.;a 2;SX;,:S 2XX ,,,7  irS02aiirBaiX:  .,ii:7,ZX7S,rZ.  8X:                                      
                                ;7Z; .2Z,X2;07;    ii,   72X7X2Z:     irXSSi;:,,ZX  r    i                                        
                                 .X:   Xr ,2rXXS,      r7:    8S    i28Zir.;Xr,  ;i                                               
                                          ,;  ia8.  ,70S  ..  22i;7r;.rBZ  ,:..,:ia                                               
                                                    :aZX...,,i  :,   .SaX    ...                                                  
### 使用模板

若想使用网站模板开发新的语音按钮，可以选择以下两种方式:

- 使用模板[模板项目](https://github.com/blacktunes/voices-button)修改
  - 修改`public`和`setting`目录下的文件以及`package.json`
- 使用[voices-button-cli](https://github.com/blacktunes/voices-button-cli)命令行工具生成项目

> 因为本项目含有非通用的代码以及访问统计，所以不推荐直接修改本仓库，若依然要使用，请注意：
>
> - 修改或删除**setting/setting.json**里用于访问统计的**GA_ID**

### LICENSE

- 项目使用**GPL-3.0**为基础开源协议
- 若使用了本项目为**范本**开发项目或使用了项目代码请在**明显位置**声明**原作者**(https://github.com/blacktunes) 以及**本仓库**(https://github.com/blacktunes/hiiro-button).
