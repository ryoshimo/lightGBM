# lightGBMを使ってみる。
環境はMacPRO pyenv(anaconda3-4.3.1)
# インストール　For OSX
https://www.analyticsvidhya.com/blog/2017/06/which-algorithm-takes-the-crown-light-gbm-vs-xgboost/

を見ると以下のようにソースコードからコンパイルしろと記述ある。

LightGBM depends on OpenMP for compiling, which isn’t supported by Apple Clang.Please use gcc/g++ instead.
-Run following:

brew install cmake

brew install gcc --without-multilib

git clone --recursive https://github.com/Microsoft/LightGBM

cd LightGBM

mkdir build 

cd build

cmake ..

make -j

私はうまく行かなかった。
pip install lightgbm
でインストールするのが簡単。
あとはjupyter上でコマンドを打つ。

# 参照
https://lightgbm.readthedocs.io/en/latest/Installation-

https://qiita.com/TomokIshii/items/3729c1b9c658cc48b5cb
