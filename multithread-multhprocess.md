# マルチスレッドとマルチプロセス

## 【事前理解】並行(Concurrent)と並列(Parallel)について

Concurrent ⊃ Parallel (※⊇かもしれない)

Concurrentは実行状態の複数保持を意味しており、Parallelは実行状態の複数保持かつ同時実行可能を意味している。

> https://twitter.com/tnmt/status/318211278810275840
> 
> 分かりやすい RT @hiboma: 羽生さんが将棋の多面指しで小学生100人を一気に相手しているのが concurrent 将棋,  羽生さんが増えて N人 (N≧2) になると parallel 将棋

シングルコア時代は並行的だった処理も、マルチコア時代になると並列的な処理が可能となった。
このことを考えるに、並行的とは、シングルコア時代の仮想的な並列処理と言うこともできる。

例えば、タイムスライスは仮想的な並列性を有している。

しかし、マルチコアの時代にも、全てを真に並列的に扱うことは出来ない。先の表現はあくまで限定的なものである。

 * [parallel と concurrent、並列と並行の違い - 本当は怖い情報科学](http://d.hatena.ne.jp/keisukefukuda/20100915/p1)
 * [第 1 章 マルチスレッドの基礎 (マルチスレッドのプログラミング)](http://docs.oracle.com/cd/E19683-01/816-3976/6ma7iosht/index.html)

### 並行的とは

```text
+-----+
| CPU | [  job1  ] [  job2  ]
+-----+
        --------------------------------------->
        time
```

### 並列的とは

```text
+------+
| CPU1 | [  job1  ]
+------+
+------+
| CPU2 | [  job2  ]
+------+
         --------------------------------------->
         time
```

 * [並行と並列について-並行コンピューティング技法-を読んで - M-Tea](http://www.m-tea.info/2011/03/concurrent-parallel-01.html)

## マルチスレッド



## マルチプロセス

