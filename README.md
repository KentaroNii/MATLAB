# 課題3レポート

「iphone.png」を原画像とする。この画像は縦616画素、横973画素の長方形のディジタルカラー画像である。

原画像を読み込み、白黒濃淡画像に変換し表示する。

・ソースコード

ORG=imread('iphone.png'); % 原画像の入力

ORG= rgb2gray(ORG); % カラー画像を白黒濃淡画像へ変換

imagesc(ORG); colormap(gray); colorbar; % 画像の表示

・結果
画像

輝度値が64以上の画素を1、64未満の画素を0とし画像を表示する。

・ソースコード

IMG = ORG > 64; % 輝度値が64以上の画素を1，その他を0に変換

imagesc(IMG); colormap(gray); colorbar;

・結果
画像

輝度値が96以上の画素を1、96未満の画素を0とし画像を表示する。

・ソースコード

IMG = ORG > 96;

imagesc(IMG); colormap(gray); colorbar;

・結果
画像

輝度値が128以上の画素を1、128未満の画素を0とし画像を表示する。

・ソースコード

IMG = ORG > 128;

imagesc(IMG); colormap(gray); colorbar;

・結果
画像

輝度値が192以上の画素を1、192未満の画素を0とし画像を表示する。

・ソースコード

IMG = ORG > 192;

imagesc(IMG); colormap(gray); colorbar;

・結果
画像

