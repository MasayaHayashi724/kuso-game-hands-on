<!-- $theme: gaia -->
<!-- footer: Masaya Hayashi -->
<!-- page_number: true -->
<!-- template: invert -->

# クソゲーを作って学ぶ
# Swift勉強会

--- 

## 今日の目的

- :x: Swiftができるようになる
- :x: ゲームが作れるようになる
- :x: クソゲーが作れるようになる
- :o: クソみたいなゲームが作れるようになる
- :o: みんな仲良くなる
- :o: Swiftが好きになる
- :o: 何か他にもアプリを作ってみたくなる

---

## お品書き

1. Swiftの簡単な文法解説 (15分)
2. ハンズオンでゲーム作ってみる (2~3時間)
3. オリジナルのゲーム作ってみる (4~5時間?)

( 4. リリースしてみる (30分~1時間) )

---

## Swiftの簡単な文法解説

### 変数定義

```swift
let height: Double = 25.5  // letは定数、再代入できない
var score: Int = 0  // varは変数、再代入できる
let nameArray: [String] = ["masaya", "hayashi"]  // 配列
var array = [1, 2, 3]  // 型が明確なら省略できる
var didWin: Bool = false  // Bool型(true, false)
let dict: [String: Int] = ["masaya": 6, "hayashi": 7]
                          // 辞書型というのもある
```

#### オプショナル型

```swift
let gender: Int? = nil
```
---

## Swiftの簡単な文法解説

#### if文

```swift
let score = 12
if score > 10 {
    print("You did it!")
} else {
    print("Try again!")
}
```

```swift
let didWin = true
if didWin {
    print("You win!")
} else {
    print("You lose...")
}
```

---

## Swiftの簡単な文法解説

#### for文

```swift
for i in 0..<10 {
    print(i)
}
```
```swift
for i in 0...10 {
    print(i)
}
```

```swift
let numbers = [1, 2, 3, 4, 5]
for number in numbers {  // for i in 0..<5 {
    print(number)        //     print(numbers[i])
}                        // }
```

---

## Swiftの簡単な文法解説

#### enumとswitch文

```swift
enum Difficulty {
    case easy
    case normal
    case hard
}
```

```swift
var difficulty: Difficulty = .normal

switch difficulty {
    case .easy: print("easy")
    case .normal: print("normal")
    case .hard: print("hard")
}
```

---

## Swiftの簡単な文法解説

### おわり

---

## 2Dゲームを作ってみよう

---

## Swift vs Unity

#### Swift (Spritekit)

- 無料で簡単
- Appleが作っている

#### Unity

- Androidも作れる
- 3Dゲームも作れる
- Asset Store

---

## では、作ってみましょう！

---

## 素材の探し方

良いフリー素材を探すのは結構時間がかかります。
あらかじめ探しておくと当日の開発がスムーズに。

#### おすすめサイト

- ぴぽや　http://blog.pipoya.net/
- illust AC　https://www.ac-illust.com/
- Rド　http://www.geocities.co.jp/Milano-Cat/3319/muz/002.html
- Folce-zero　http://folce.zatunen.com

---

## シューティングゲームを作る

1. プロジェクトの作成
2. メニュー画面とゲーム画面の作成
3. 宇宙船を追加 (傾けると移動、タップでミサイル)
4. 小惑星を追加 (ランダム位置に出現して迫ってくる)
5. 衝突処理 (ミサイルと小惑星、小惑星と宇宙船)
6. スコアとライフを導入
7. ゲーム終了処理
8. ベストスコアの保存

---

## 実機でビルドする方法

- http://qiita.com/DKN915/items/7a2ce97f3758e2daf486
- 上の記事を参考にしてね。

---

## 好きなゲームを作ってみよう！

---

## 作ったゲームをリリースする

- 時間があればやりましょう
- 後日やっても大丈夫です
