# 課題7レポート

「iphone.png」を原画像とする。この画像は縦616画素、横973画素の長方形のディジタルカラー画像である。

原画像を読み込み、白黒濃淡画像に変換し表示する。

・ソースコード

ORG = imread('iphone.png'); % 画像の読み込み

ORG = rgb2gray(ORG); % 白黒濃淡画像に変換

imagesc(ORG); colormap(gray); colorbar; % 画像の表示

・結果
画像

原画像のヒストグラムを表示する。

・ソースコード

imhist(ORG); % 濃度ヒストグラムを生成、表示

・結果
画像

ダイナミックレンジを0から255に拡張し、画像を表示する。

・ソースコード

ORG = double(ORG);

mn = min(ORG(:)); % 濃度値の最小値を算出

mx = max(ORG(:)); % 濃度値の最大値を算出

ORG = (ORG-mn)/(mx-mn)*255;

imagesc(ORG); colormap(gray); colorbar; % 画像の表示

・結果
画像

ダイナミックレンジを拡張した後の画像のヒストグラムを表示する。

・ソースコード

ORG = uint8(ORG); % この行について考察せよ

imhist(ORG); % 濃度ヒストグラムを生成、表示

・結果
画像
