# 共有ライブラリlibhello.soを作成する
$ g++ -shared src/hello.cpp -o libhello.so
  
# 作成した共有ライブラリを使用する
$ g++ main.cpp ./libhello.so
  
# コンパイルしたファイルを実行する
$ ./a.out
  
# libhello.soを削除した後に ./a.outをすると下記のエラーになる
error while loading shared libraries: ./libhello.so: cannot open shared object file: No such file or directory
