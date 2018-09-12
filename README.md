# Akrep MD5 Cracker

[![N|Solid](https://emregeldegul.net/wp-content/uploads/2018/09/akrepUsage.png)]( https://emregeldegul.net/2018/09/akrep-md5-cracker/)

Akrep, daha önce farklı bir grup için yazdığım online, wordlist ve random seçenekleri ile MD5 hashleri çözmeye çalışan küçük bir program. Henüz kendimi geliştirdiğim dönemlerde yazdığım bir program, piyasada daha güçlü programlar da mevcut. Ama sizlerin işine yarayabileceğini düşünüyorum.

## Program Kurulum
Programı git ile klonlayabilirsiniz.
```sh
~$ git clone https://github.com/MuReCoder/akrep.git
```

## Program Kullanım
Komut satırından, indirdiğiniz dizine gelip "python md5cracker.py" diyerek yardım menüsüne ulaşabilirsiniz.

```sh
~$ python md5cracker.py
```

### Online Tarama
Online tarama için hash ile beraber -o parametresi ile -pass argümanı gönderilir.

```sh
~$ ./md5cracker.py d8578edf8458ce06fbc5bb76a58c5ca4 -o -pass
```

[![N|Solid](https://emregeldegul.net/wp-content/uploads/2018/09/akrepOnlineEx.png)]( https://emregeldegul.net/2018/09/akrep-md5-cracker/)

### WordList Tarama
Wordlist tarama için -w parametresi ile wordlist dosyası argüman olarak gönderilir.

```sh
~$ ./md5cracker.py d8578edf8458ce06fbc5bb76a58c5ca4 -w /root/wordlist.py
```
### Random Tarama
Random tarama için -r parametresi ile beraber karakter aralığı gönderilir. Bu random üretilecek karakterlerin hangi sayı aralığında olacağını belirler. Örneğin 2,8. bu en az 2 en fazla 8 karakterlik kelime üretecek demektir.

```sh
~$ ./md5cracker.py d8578edf8458ce06fbc5bb76a58c5ca4 -r -2,8
```
