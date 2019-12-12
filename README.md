# pie-kirari

https://twitter.com/piepielielie/status/1204747955963494402

## 喋ってもらう

オマケ機能として `$ docker-compose up` 時に「docker-compose up」と喋ってもらうことができます．

- 使用中のターミナルでの `$PATH` が汚れるので，注意してください．(ターミナルを開き直すと直ります)
- Mac のみ動作確認しています．Windowsだと動かないと思います．
- audio.m4a は自分で用意してください

```bash
# docker-compose コマンドが書き換わっているのを試したい方
$ source ./setup
$ docker-compose up
Starting pie-kirari_hello_1 ... done
Attaching to pie-kirari_hello_1
hello_1  |starting process... pie ki-rari
```

```bash
# これでも動くんだけどね
$ PATH=$(pwd):$PATH docker-compose up
```