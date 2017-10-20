# NodeJS 8  Vangrant Box

Clone the repo and run the following (ensure you have VirtualBox and Vagrant installed):
```
vagrant up
```

After install:

```
vagrant status
vagrant ssh
``` 

В процессе будет закачан образ ВМ с Убунту - осторожно, это занимает мегабайты.

В файле настройки Вагранта есть `config.vm.network "forwarded_port", guest: 3000, host: 3000` - это открытие порта наружу из виртуальной машины.

Соответственно, внутри машины можно запустить что-то на порту 3000 и открывать это на хост-машине: localhost:3000
