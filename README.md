Pythonのメモ
パッケージマネージャ：pip
仮想環境：virtualenv
参考にしたサイト：http://study-flask.readthedocs.org/ja/latest/01.html

shell

mkdir PythonFlask01
cd PythonFlask01
virtualenv env
env\Scripts\activate.bat
pip install Flask

./configure
ソースファイルをコンパイルする前に、インストール対象となるシステム特有の機能
情報をチェックし、チェック状況を記述したMakefileを作成する。

configureに失敗する場合は、コンパイルに必要なライブラリ、
ヘッダファイル等が不足している事がほとんどなので、
エラーメッセージの内容を確認し、必要なパッケージを事前に
インストールしておく。

make
configureの実施により作成されたMakefileを元に、
以下のようにmakeコマンドを実行することで、ソースファイルのコンパイルを行う。
コンパイル時にエラーが表示されるようであれば、エラー内容を確認し、
configure実行時に必要なパラメータが不足していないか確認する。

make install
make実行時にエラーが表示されなければコンパイル完了である
（コンパイル途中に警告メッセージが表示される場合があるが、これは無視してもOK）
コマンドでインストール
(make で作成したファイルなどを任意のディレクトリにコピー)を行う。
