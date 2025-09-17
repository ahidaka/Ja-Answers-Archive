# Windows 11 24H2 の利用とトラブル対応 - Microsoft コミュニティ

Windows 11 24H2 が Windows Insider Canary チャネルと Dev チャネルで公開中ですが、トラブル関連の質問が増えて来たので整理してお知らせします。

まず Windows Insider はリリース版ではありせん。新機能を確認し、[フィードバックを送る](https://aka.ms/WIPFeedbackHub) ための評価版です。つまり人柱用です。人柱とは「命を投げ出す、犠牲になる、捨て石となる、献身する」ことです。その覚悟が無い方は利用しない方がいいでしょう。したがってトラブル発生時は、次の手順でフィードバックして、必要に応じて再インストールをします。ご自身で問題解決に取り組むことや、ここでのトラブル情報の交換は出来ますが、**更新頻度が多い事前評価版なのでサポートはありません。**

**トラブル対応方法**

１．[**フィードバック Hub **](https://support.microsoft.com/ja-jp/windows/%E3%83%95%E3%82%A3%E3%83%BC%E3%83%89%E3%83%90%E3%83%83%E3%82%AF-hub-%E3%82%A2%E3%83%97%E3%83%AA%E3%82%92%E4%BD%BF%E3%81%A3%E3%81%A6-microsoft-%E3%81%AB%E3%83%95%E3%82%A3%E3%83%BC%E3%83%89%E3%83%90%E3%83%83%E3%82%AF%E3%82%92%E9%80%81%E4%BF%A1%E3%81%99%E3%82%8B-f59187f8-8739-22d6-ba93-f66612949332)でトラブルを報告

２．インストールメディアの作成とマウント（リリース版の再インストール）

[**Windows 11 をダウンロードする**](https://www.microsoft.com/ja-jp/software-download/windows11) から MediaCreationTool_Win11_23H2.exe または ISOファイルを作成またはダウンロードしてマウントします。

３．「個人データ」も「アプリ」も、すべてを引き継がない「新規インストール」（以外は選択不可）

マウントしたISOファイルの中にある「setup.exe」を起動して実行。個人データもアプリも、「何もしない」（引き継がない）新規インストールを実行します。

４．リリース版のインストール完了後、参加チャネルを選択し直して再度参加することや、Insider から離脱することが可能です。

**インストール方法**

１．参加用PCの用意

Windows 11 が正常動作している、「いつでもクリーンな再インストールが可能」なPCを、**メインで使用しているPCとは別に Insider 参加用に **用意します。

２．チャネル選択

そのPCで Microsoftアカウントにサインインして、Windows Update の **Windows Insier Program** のメニューから、購読チャネルを「Devチャネル」か「Canaryチャネル」を選択して、Insider Program に参加します。「Beta チャネル」と「Release Preview (RP) チャネル」も参加可能です。**6月15日から一部のRelease Preview (RP) チャネルで 24H2 配布が開始されました**が、確実に 24H2 をインストールするのであれば、Devチャネル以上に参加します。勿論、より安定版でのインストールを狙うのであれば、 コメントの通りRP チャネル登録を先に試して「24H2が降りてくるのを待つ」方法や、24H2 RP ISOインストールもあります。

[![画像]("Windows 11 24H2 の利用とトラブル対応 - Microsoft コミュニティ_files"/58eba207-c305-47fc-a76b-faf639fa9d35.png)]("Windows 11 24H2 の利用とトラブル対応 - Microsoft コミュニティ_files"/58eba207-c305-47fc-a76b-faf639fa9d35.png)

.

「最小ハードウェア要件を満たしていない」PC でもTPM 1.2または TPM 2.0 を搭載していれば参加できます。下記の警告が出ます。

Hyper-V 等の仮想マシンのゲストOSでも、TPMが有効化してあれば参加できます。

[![画像]("Windows 11 24H2 の利用とトラブル対応 - Microsoft コミュニティ_files"/eddf50a2-4813-4921-8a6d-e926746c1685.png)]("Windows 11 24H2 の利用とトラブル対応 - Microsoft コミュニティ_files"/eddf50a2-4813-4921-8a6d-e926746c1685.png)

.

３．Windows Update で 24H2 をインストール

そのままでは、１～２日程度待たないと「24H2」のインストールが始まらない場合があります。おかしいと感じたらば、２～３分程度待ちながら、繰り返し Windows Update を実行します。

追記）

6月15日から Release Preview (RP)チャネルで 24H2 配布が始まったため、一部修正しました。

参考の質問）

[**２４Ｈ２をインストールしたいので、やり方を教えてください。 **](https://answers.microsoft.com/ja-jp/insider/forum/all/%EF%BC%92%EF%BC%94%EF%BD%88%EF%BC%92%E3%82%92/244b19f4-12ba-4bbe-aaf0-b0a6f546cd43)

[**Insider Preview登録してあるのにBeta版にアップグレードできない**](https://answers.microsoft.com/ja-jp/insider/forum/all/insider/4eaef489-f3f4-4944-82e9-e1c657175c18)

勘違い質問の例）

[Windows のオーディオに関する問題のトラブルシューティング](https://answers.microsoft.com/ja-jp/insider/forum/all/windows/716dfac9-6bf8-407e-a559-18fb4204f2b5)

[緑の画面にWindows Insider ビルドに問題が発生し、再起動する必要があります。 エラー情報を収集しています。自動的に再起動します。](https://answers.microsoft.com/ja-jp/insider/forum/all/%e7%b7%91%e3%81%ae%e7%94%bb%e9%9d%a2%e3%81%abwindo/f80c3c6a-695d-4849-b214-e6da64dd867d)

[アップデートができません](https://answers.microsoft.com/ja-jp/insider/forum/all/%e3%82%a2%e3%83%83%e3%83%97%e3%83%87%e3%83%bc/67c03b3a-baf8-4161-a5af-404486f11a4b)

[アップデートがエラーになって困っております](https://answers.microsoft.com/ja-jp/insider/forum/all/%e3%82%a2%e3%83%83%e3%83%97%e3%83%87%e3%83%bc/1bcd4be6-d2ae-4295-ba77-d244de47787a)

[関連付け・スタートなど不具合が多発する。](https://answers.microsoft.com/ja-jp/insider/forum/all/%E9%96%A2%E9%80%A3%E4%BB%98%E3%81%91%E3%82%B9/b6453ee6-174b-4362-86e5-aab14833923c)

追記）

この記事は随時更新しますので、情報があればコメントをお願いします。
