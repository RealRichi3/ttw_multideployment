(rr-ci)=
# 継続的統合

| 前提条件                                                                     | 重要度       | メモ                                                        |
| ------------------------------------------------------------------------ | --------- | --------------------------------------------------------- |
| [コマンドラインでの経験](https://programminghistorian.org/en/lessons/intro-to-bash) | 必要な       | 継続的インテグレーションはコマンドラインの指示に従います                              |
| {ref}`バージョンコントロール<rr-vcs>`                                         | 必要な       | 新しい _コミット_ がプロジェクトに行われるたびに連携が実行されます。                      |
| {ref}`再現可能な計算環境<rr-renv>`                                          | 必要な       | 継続的な統合では、テストは別のコンピュータ(通常はクラウド)で実行されますので、同じ方法で設定する必要があります。 |
| {ref}`テスト<rr-testing>`                                             | とても役に立ちます | プロジェクトを変更したときに重要なことが変更された場合、継続的な統合 _テスト_                  |

## Summary

継続的インテグレーション(CI)は、個人が行ったプロジェクトへの変更をメインに統合する方法です。 頻繁に共有されているバージョン(通常は1日に複数回)。 CI ソフトウェアは、通常、変更によって導入された競合やバグを特定するためにも使用されます。 彼らは見つけて早期に固定されるので必要な労力を最小限に抑えることができます 定期的にテストを実行すると、人々が手動でそれを行う必要がなくなります。 定期的にテストを実行すると、人々が手動でそれを行う必要がなくなります。 ユーザーにバグをできるだけ早く認識させることによって(プロジェクトが研究プロジェクトの場合)、捨てなければならない作業に多くの時間を費やすことはありません。 テストが頻繁に実行されず、結果が不完全なコードを使用して生成される場合に該当する可能性があります。

```{figure} ../figures/continuous-integration-may19.*
---
height: 500px
name: continuous-integration-may19
alt: 開発者の計画にどのように継続的な統合が役立つかを示すスケッチ。
---
_Scriberiaによるチューリング方法_プロジェクトのイラスト。 CC-BY 4.0ライセンスの下で使用される。 DOI: [10.5281/zenodo.3332807](https://doi.org/10.5281/zenodo.3332807)
```

## モチベーションと背景

CI にはいくつかの重要な利点があります。

- バグの早期発見を支援し、ダメージを最小限に抑え、修正を容易にします
- プロジェクトの貢献者をお互いの仕事で最新の状態に保ち、できるだけ早く利益を得られるようにします
- ユーザーにテストを書くように促します
- テストの実行を自動化
- テストが頻繁に実行されることを保証します
