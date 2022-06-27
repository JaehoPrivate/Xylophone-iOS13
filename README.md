# Xylophone 수업으로 배운 점 및 원자료

## 실습으로 배운 점
* AVFoundation, AVAudioPlayer를 이용해 음악 파일을 재생하는 방법.
* 본인이 모르는 기능을 앱에서 구현하고 싶을 때 Google 검색하는 방법 및 Stackover Flow 등으로 스스로 학습하는 방법.
* Button의 타이틀과 각 음별 음악파일 이름을 동일하게 설정해서 버튼이 클릭될 때마다 소리가 재생되도록 설정 

## 수업 원자료는 아래와 같음

![App Brewery Banner](Documentation/AppBreweryBanner.png)

# Xylophone

## Our Goal

The goal of this tutorial is to dive into a simple iOS recipe - how to play sound and use an Apple library called AVFoundation. The most important skill of a great programmer is being able to solve your own problems. We’ll do that by exploring StackOverflow, Apple Documentation and learning how to search for solutions effectively. By learning to use these tools, you’ll be able to start adding custom features to an app and get it to do what you want it to.


## What you will create

You will be making your first musical instrument! Music apps are so popular on the App Store that they even get their own category. So in this module, we’re going to make a colourful XyloPhone app. Get it? Ok, the jokes are bad, but remember, I only wrote the good ones... 

## What you will learn

* How to play sound using AVFoundation and AVAudioPlayer.
* Understand Apple documentation and how to use StackOverflow.
* Functions and methods in Swift. 
* Data types.
* Swift loops.
* Variable scope.
* The ViewController lifecycle.
* Error handling in Swift.
* Code refactoring.
* Basic debugging.

## Replacement Code

```
import UIKit
import AVFoundation

class ViewController: UIViewController {
    
    var player: AVAudioPlayer!

    override func viewDidLoad() {
        super.viewDidLoad()
    }

    @IBAction func keyPressed(_ sender: UIButton) {
        playSound()
    }
    
    func playSound() {
        let url = Bundle.main.url(forResource: "C", withExtension: "wav")
        player = try! AVAudioPlayer(contentsOf: url!)
        player.play()
                
    }
}
```



>This is a companion project to The App Brewery's Complete App Development Bootcamp, check out the full course at [www.appbrewery.co](https://www.appbrewery.co/)

![End Banner](Documentation/readme-end-banner.png)

