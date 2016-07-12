# Stanford_iOS_Lecture_DemoBundle

First of all, thanks for Stanford University gave us such a great open class : [Developing Apps for iOS CS193P](https://itunes.apple.com/WebObjects/MZStore.woa/wa/viewPodcast?id=480479762).

This DemoBundle contains the demo which were taught in this class.

I summarize these lectures in my Chinese blog in [JianShu](http://www.jianshu.com/users/3dd433cb3ea1/latest_articles). While, I do not have summarized all the lectues yet, so you can not see all of the demos. But I will continue to summarize and present the demo to you.

And there are two parts of this bundle, one contains the code with Chinese note which is easy to be understood by Chinese-speaking friends. Another part has English note for western friends.

##Note Examples


###Code with English note:

```       
    //1. card front
    //1.1 card front middle image
    UIImage *faceImage = [UIImage imageNamed:[NSString stringWithFormat:@"%@%@",[self rankAsString],self.suit]];
    
    if (faceImage) {
        
        CGRect imageRect = CGRectInset(self.bounds, self.bounds.size.width * (1.0 - self.faceCardScaleFactor) + 20, self.bounds.size.height * ( 1.0 - self.faceCardScaleFactor  ) + 20);
        [faceImage drawInRect:imageRect];
    }
    
    //1.2 draw card corners
    [self drawCorners];
    
}else{
    
    //2. set card back image
    [[UIImage imageNamed:@"cardBack"] drawInRect:self.bounds];


```

###Code with Chinese note:

```
    //1. 纸牌正面
    //1.1 纸牌正面中间的图
    UIImage *faceImage = [UIImage imageNamed:[NSString stringWithFormat:@"%@%@",[self rankAsString],self.suit]];
    
    if (faceImage) {
        
        CGRect imageRect = CGRectInset(self.bounds, self.bounds.size.width * (1.0 - self.faceCardScaleFactor) + 20, self.bounds.size.height * ( 1.0 - self.faceCardScaleFactor  ) + 20);
        [faceImage drawInRect:imageRect];
    }
    
    //1.2 纸牌正面四个角
    [self drawCorners];
    
    }else{
    
    //2. 纸牌背面
    [[UIImage imageNamed:@"cardBack"] drawInRect:self.bounds];

    
```


##Demo Examples

###Card Matching Game

![image](https://github.com/Shijie0111/Stanford_iOS_Lecture_DemoBundle/blob/master/Resources/card.gif)


###Drop it
![image](https://github.com/Shijie0111/Stanford_iOS_Lecture_DemoBundle/blob/master/Resources/drop.gif)

There maybe some bugs, but I think we can make this be better and better!
Wecome to download and discuss with me!

Thanks again for Stanford University.