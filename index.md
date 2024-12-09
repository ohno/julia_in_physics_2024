---
title: Julia in Physics 2024
description: Juliaは2018年にバージョン1が公開されたオープンソースの科学技術計算言語で, Fortranの様に高速でかつPythonの様に生産性の高い言語である. Julia は様々な分野において活用が始まっている. 本研究会では, 主に基礎科学においてのJulia の使用例などを議論する. また可視化, 高速計算, 微分方程式の数値解法, 統計・機械学習分野への応用例や実装例, パッケージ開発も議論の対象とする. 研究機関に所属する研究者だけでなく産業界での研究者, 学生などの積極的な参加を歓迎する.
---

<script type="text/x-mathjax-config">
  MathJax.Hub.Config({
      extensions: ["tex2jax.js"],
      tex2jax: {
          inlineMath: [ ['$','$'], ["\\(","\\)"] ],
          processEscapes: true,
          processRefs: true,
          processEnvironments: true
      },
      TeX: { equationNumbers: { autoNumber: "AMS" } }
  });
</script>
<script type="text/javascript" async
  src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML">
</script>

# 概要

下記の要綱にて Julia in Physics 2024 を開催します. 皆様のご参加をお待ちしております.

| **日時**     | 2024年12月14日(土) 13:00 - 19:00 |
| **開催方式** | 対面 / Zoom ハイブリット |
| **会場**     | [東京大学 本郷地区キャンパス(浅野キャンパス) 情報基盤センター(本館) 214](#アクセス) |
| **最寄り駅** | 根津駅（千代田線） |
| **申し込み** | [https://forms.gle/WTiyPtf97Q2LcDA59](https://forms.gle/WTiyPtf97Q2LcDA59) |

# プログラム

プログラムは予告なく変更される可能性があります. 

| **12:45 -**       | 開場, ※開場前は施錠されているため建物には入れません |
| **13:00 - 13:10** | 開会のあいさつ, 諸連絡 |
| **13:10 - 14:10** | [招待講演１](#招待講演１)（数値計算）|
|                   | 休憩 |
| **14:10 - 15:10** | [招待講演２](#招待講演２)（HPC） |
|                   | 休憩, 集合写真 |
| **15:40 - 16:40** | [招待講演３](#招待講演３)（テンソルネットワーク）|
|                   | 休憩 |
| **16:50 - 17:05** | [一般講演１](#一般講演１) |
| **17:05 - 17:30** | [一般講演２](#一般講演２) |
|                   | 休憩 |
| **17:40 - 18:05** | [一般講演３](#一般講演３) |
| **18:05 - 18:30** | [一般講演４](#一般講演４) |
| **18:30 - 18:40** | 閉会のあいさつ |
| **19:00 -**       | 懇親会 |

## 招待講演１

| **題目** | Juliaによる数値計算入門 |
| **氏名** | 永井 佑紀 |
| **所属** | 東京大学 情報基盤センター |
| **概要** | TBA |

## 招待講演２

| **題目** | Productivity meets performance: Julia for HPC |
| **氏名** | Valentin Churavy |
| **所属** | Johannes-Gutenberg University Mainz & University of Augsburg |
| **概要** | Julia is a flexible, friendly, fast programming language for scientific (and beyond) computations. This talk will discuss benefits and challenges of using Julia in HPC, particularly on  Fujitsu A64FX ARM-based processors. The flexibility of Julia makes it particularly well-suited to take advantage of the interesting combination of hardware features of A64fx, such as Scalable Vector Extension (SVE), and native support for reduced-precision floating-point arithmetic. I will discuss the compilation pipeline using  a performance study, demonstrating that Julia can match the performance of tuned libraries. |

## 招待講演３

| **題目** | 関数のテンソルトレイン表現をjuliaで入門 |
| **氏名** | 櫻井 理人 |
| **所属** | 日本学術振興会特別研究員PD<br>東京大学大学院理学系研究科藤堂研究室 |
| **概要** | テンソルネットワークはもともと量子状態の圧縮のために発展してきたが、応用数学の分野では幅広い関数系の圧縮へ応用されている。ここでは応用数学で発展した圧縮技術であるTensorCrossInterpolationに焦点を当て、Juliaで開発された[TensorCrossInterpolation.jl](https://github.com/tensor4all/TensorCrossInterpolation.jl)を扱う。TensorCrossInterpolation.jlとITensors.jlの使い方のデモを交えつつ、関数のテンソルトレイン表現と演算、その応用例についても触れる。 |

## 一般講演１

| **題目** | 3D-BOS法による流体密度場の3次元再構成コードのJuliaでの開発 |
| **氏名** | 赤嶺　政仁 |
| **所属** | 東京大学大学院 工学系研究科 航空宇宙工学専攻 講師 |
| **概要** | 超音速乱流ジェットなどの複雑な流体現象を、３次元・非接触で計測できる「3D-BOS法」のためのコード開発をJuliaで進めている。CUDA.jlでの高速化なども行っているので、その事例を紹介したい。（https://doi.org/10.1007/s00348-023-03672-1 で既報の内容を含む。コードはhttps://github.com/wavepackets/SchlierenReconstructions.jl で公開準備中） |

## 一般講演２

| **題目** | Machine Learning Estimation on the Trace of Inverse Dirac Operator using the Gradient Boosting Decision Tree Regression |
| **氏名** | Benjamin J. Choi |
| **所属** | 筑波大学計算科学研究センター |
| **概要** | We present our preliminary results on the machine learning estimation of $\mathrm{Tr}~M^{-n}$ from other observables with the gradient boosting decision tree regression, where $M$ is the Dirac operator. Ordinarily, $\mathrm{Tr}~M^{-n}$ is obtained by linear CG solver for stochastic sources which needs considerable computational cost. Hence, we explore the possibility of cost reduction on the trace estimation by the adoption of gradient boosting decision tree algorithm. We also discuss effects of bias and its correction. |

## 一般講演３

| **題目** | Juliaではじめる変分法 |
| **氏名** | 大野 周平 |
| **所属** | 横浜市大学大学院 生命ナノシステム科学研究科 物質システム科学専攻 量子物理化学研究室 D2<br>理化学研究所 仁科加速器研究センター 少数多体系物理研究室 大学院生リサーチ・アソシエイト（JRA） |
| **概要** | J.M.ティッセン著『計算物理学』(丸善出版, 2012)の第3章を参考に, Schrödinger方程式に対する変分法について解説する. ガウス型基底関数による水素原子の変分計算を演習形式で解説し, Juliaによる実装を例示する. 実用的な例として[TwoBody.jl](https://ohno.github.io/TwoBody.jl/)によるクォーク模型（チャーモニウムの質量）の計算を実演し, 最後に三体系以上への拡張に向けた課題と展望を述べる. |

## 一般講演４

| **題目** | Juliaではじめる格子QCD |
| **氏名** | 富谷 昭夫 |
| **所属** | 現代教養学部 数理科学科 情報数理科学専攻 専任講師 |
| **概要** | TBA |

# 参加登録

[こちらのフォーム](https://forms.gle/WTiyPtf97Q2LcDA59)よりご登録ください.

# アクセス

最寄り駅は **根津駅 (千代田線)** です. **情報基盤センター(本館) 214** までお越しください.

<iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3239.4161578803523!2d139.76245279855846!3d35.71598244584945!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x60188c2e4e11be15%3A0xdfb3af990c344d7d!2z44CSMTEzLTAwMzIg5p2x5Lqs6YO95paH5Lqs5Yy65byl55Sf77yS5LiB55uu77yR77yRIOaDheWgseWfuuebpOOCu-ODs-OCv-ODvCjmnKzppKgp!5e0!3m2!1sja!2sjp!4v1731924110887!5m2!1sja!2sjp" width="600" height="450" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>

# 当日レポート

Xのハッシュタグは[`#JuliaInPhysics2024`](https://twitter.com/hashtag/JuliaInPhysics2024)です.

<a href="https://twitter.com/intent/tweet?button_hashtag=x&ref_src=twsrc%5Etfw" class="twitter-hashtag-button" data-show-count="false">Tweet #x</a><script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>

# お問い合せ

[こちらのフォーム](https://forms.gle/WTiyPtf97Q2LcDA59)に記載のメールアドレスよりご連絡ください.

# リンク

Julia言語について

- [Julia公式サイト](https://julialang.org/)
- [なぜ僕らはJuliaを作ったか](https://www.geidai.ac.jp/~marui/julialang/why_we_created_julia/index.html)

関連イベント

- [Julia in Physics 2021 Online](https://akio-tomiya.github.io/julia_in_physics/)
- [数学と物理におけるJuliaの活用](https://akio-tomiya.github.io/julia_imi_workshop2023/)

世話人（順不同）

- 大野 周平（横浜市立大学, 理化学研究所）
- 富谷 昭夫（東京女子大学）
- 永井 佑紀（東京大学）
- 大野 浩史（筑波大学）

本研究会は[科学研究費補助金学術変革領域研究(A)「学習物理学の創成」](https://mlphys.scphys.kyoto-u.ac.jp/)の支援を受けた.
