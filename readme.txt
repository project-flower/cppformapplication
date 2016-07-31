Visual Studio 2015でCPP/CLIでWindows フォーム アプリケーションを作成するプロジェクト テンプレート

使用方法:
以下のファイルを
%USERPROFILE%\Documents\Visual Studio 2015\Templates\ProjectTemplates\cppformapplication
にコピーする事で、新しいプロジェクトのVisual C++にcppformapplicationが追加されます。

問題:
項目"CLR"の中に表示されて欲しいのだが、表示されない。
ユーザーが選択したターゲット フレームワークが反映できない。$clrversion$ではダメだった。現状v3.5固定にしている。
.vcxprojの<PropertyGroup Label="Globals">内のTargetFrameworkVersionを変更する事で一応変更はできるが、
v2.0等を指定するとデザイナ編集時にエラー。.resxファイル内のバージョンも4.0.0.0になってしまう。
(C++/CLIでv2.0はVS2015では利用できない？)
