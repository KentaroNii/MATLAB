# 課題6レポート

「iphone.png」を原画像とする。この画像は縦616画素、横973画素の長方形のディジタルカラー画像である。

原画像を読み込み、白黒濃淡画像に変換し表示する。

・ソースコード

ORG=imread('iphone.png'); % 原画像の入力

ORG = rgb2gray(ORG);

imagesc(ORG); colormap(gray); colorbar; % 画像の表示

・結果
画像

色を128で2段階に分けて画像を二値化し、表示する。

・ソースコード

IMG = ORG>128; % 128による二値化

imagesc(IMG); colormap(gray); colorbar; % 画像の表示

・結果
画像

ディザ法を用いて画像を二値化し、表示する。

・ソースコード

IMG = dither(ORG); % ディザ法による二値化

imagesc(IMG); colormap(gray); colorbar; % 画像の表示

・結果
画像
