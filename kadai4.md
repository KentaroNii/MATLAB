# 課題4レポート

「iphone.png」を原画像とする。この画像は縦616画素、横973画素の長方形のディジタルカラー画像である。

原画像を読み込み、白黒濃淡画像に変換し表示する。

・ソースコード

ORG=imread('iphone.png'); % 原画像の入力

ORG=rgb2gray(ORG); % カラー画像を白黒濃淡画像へ変換

imagesc(ORG); colormap(gray); colorbar;

・結果
画像

原画像のヒストグラムを表示する。

・ソースコード

imhist(ORG); % ヒストグラムの表示

・結果
画像
