# 2024GSC_SatoAki2 中間発表 『富士山3Dモデル生成のためのPythonライブラリ開発提案』

## 1. はじめに（Introduction）

富士山は日本を代表する山岳であり、その詳細な3Dモデルは防災、観光、教育など多岐にわたる分野での活用が期待されている。しかし、富士山の高精度な3Dモデルを容易に取得・操作・可視化するための統合的なツールは限られている。本提案では、国土交通省のPLATEAUプロジェクトが提供するオープンデータを活用し、富士山周辺の詳細な3Dモデルを生成・操作するPythonライブラリの開発を目指す。

## 2. 先行研究（Background）

PLATEAUプロジェクトは、日本全国の3D都市モデルをオープンデータとして提供しており、これらのデータを活用するためのツールやライブラリも開発されている。例えば、PlateauKitはPLATEAUの3D都市モデルを扱うためのPythonライブラリであり、データの変換や可視化をサポートしている。 また、PlateauUtilsは3D都市モデル（CityGML・3DTiles/MVT）をパースして、Pythonに読み込むためのライブラリである。 しかし、これらのツールは主に都市部のデータを対象としており、富士山のような山岳地帯の詳細な3Dモデル生成に特化したものではない。

他の先行事例として、PythonとPlotlyを用いて富士山の立体図をブラウザ上で表示する手法がある。 また、Panda3Dライブラリを使用して3D地図を作成する方法も報告されている。 これらの事例は、特定のツールやライブラリを用いて3Dモデルを生成・可視化するものであり、汎用的なPythonライブラリとしての提供は行われていない。

参考にした資料のURLは、参考文献欄に記載している。

## 3. 方法（Method)

本プロジェクトでは、以下のステップで富士山の3Dモデル生成ライブラリを開発する予定である。

1. **データ収集:** PLATEAUプロジェクトのオープンデータポータルから、富士山地域の3D都市モデルデータを収集する。
2. **データ処理:** 収集したデータを前処理し、必要に応じてCityGMLから他の形式（例: GeoJSON）への変換を行う。
3. **モデル生成:** 前処理したデータを基に、富士山の高精度な3Dモデルを生成する。
4. **可視化:** 生成した3DモデルをPython環境で可視化し、ユーザーが容易に操作・解析できるようにする。

## 4. 結果（Results）

開発されたライブラリにより、ユーザーは以下の機能を利用できる。

- 富士山の詳細な3Dモデルの自動生成
- 生成モデルのインタラクティブな可視化
- 地形解析や断面図の生成などの地理空間解析機能

## 5. 考察（Discussion）

本ライブラリは、研究者、教育者、開発者が富士山の3Dデータを活用したプロジェクトを迅速に開始できる環境を提供する。また、PLATEAUプロジェクトのデータを活用することで、高精度なモデル生成が可能となり、地形解析やシミュレーションの効率化が期待される。さらに、他の山岳地帯や地域への適用も視野に入れ、汎用性の高いツールとしての発展が見込まれる。

## 6. 結論（Conclusion）

富士山の3Dモデル生成に特化したPythonライブラリの開発は、地理空間データの活用を促進し、多様な分野での応用が期待される。PLATEAUプロジェクトのオープンデータを最大限に活用し、ユーザーが容易に高精度な3Dモデルを生成・操作・解析できる環境を提供することを目指す。 


## 参考文献（References）
PlateauKit:https://github.com/ozekik/plateaukit
<br/>PlateauUtils:https://github.com/Project-PLATEAU/PlateauUtils
<br/>PythonとPlotlyで富士山の立体図をブラウザ上で表示する:https://www.odndo.com/posts/python-plotly-html-fujisan/
<br/>Pythonで複数の標高タイルを結合して富士山の3D立体地形図を描いてみる:https://memomemokun.hateblo.jp/entry/2018/11/30/204618
<br/>Project-PLATEAU/Auto-Create-bldg-lod2-tool:https://github.com/Project-PLATEAU/Auto-Create-bldg-lod2-tool
