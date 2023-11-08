```mermaid
graph LR;
    A-->B;
    A-->C;
    B-->D;
    C-->D;
```
```mermaid
flowchart BT
    id1["銀行でお金をおろす"]
    id2["ゆで卵を作る
    作業時間10分"]
    id1 ==10分待ちなさい==> id2
```

```mermaid
flowchart TB
    c1-->a2
    subgraph one
    a1-->a2
    end
    subgraph two
    b1-->b2
    end
    subgraph three
    c1-->c2
    end
```

```mermaid
flowchart TD
    id1["ゆで卵を食べる"]
    subgraph "(第二階層)大まかな計画"
    id2[卵を買う]
    id3[ゆで卵を作る]
    id4[食べる準備をする]
    end
    subgraph "(第三階層)アクテビティ"
    id5[銀行で金をおろす]
    id6[スーパーで卵を買う]
    id7[卵を洗う]
    id8[お湯を沸かす]
    id9[卵をゆでる]
    id10[腹筋して腹をへらす]
    id11[殻を割る]
    id12[塩を振る]
    end


    id1-->id2
    id1-->id3
    id1-->id4
    id2-->id5
    id2-->id6
    id3-->id7
    id3-->id8
    id3-->id9
    id4-->id10
    id4-->id11
    id4-->id12
```
```mermaid
flowchart LR
    id1["銀行で金をおろす
    作業時間 10分"]
    id2["スーパーで卵を買う
    作業時間 10分"]
    id3["卵を洗う
    作業時間 10分"]
    id4["お湯を沸かす
    作業時間 20分"]
    id5["卵をゆでる
    作業時間 10分"]
    id6["卵を割る
    作業時間 10分"]
    id7["塩を振る
    作業時間 10分"]
    id8["腹筋して腹をへらす
    作業時間 30分"]
    id1 --> id2
    id2 --> id3
    id4 --> id5
    id5 --> id6
    id6 --> id7
    id3 --> id5
```

| アクテビティ | 担当 |  |  |  |
| --- | --- | --- | --- | --- |
| 銀行で金をおろす | 太郎 | #008000 |  |  |  |
| スーパーで卵を買う | 太郎 |
| 卵を洗う | 太郎 |
| お湯を沸かす | 花子 |
| 卵をゆでる | 花子 |
| 腹筋して腹をへらす | 太郎 |
| 殻を割る | 花子 |
| 塩を振る | 花子 |