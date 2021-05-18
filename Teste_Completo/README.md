## Instale o gpiozero

```
sudo apt update
sudo apt install python3-gpiozero
```

#### Copie o arquivo main.py para /home/pi/myscript

#### Copie o arquivo myscript.service para /etc/systemd/system

#### Habilite a iniciação automática do serviço

```
sudo systemctl enable myscript.service
```

#### Inicie o serviço
```
sudo systemctl start myscript.service
```

#### Se acontecer algum problema de permissão, mude as permissões dos arquivos

```
sudo chmod 755 /home/pi/myscript/main.py
sudo chmod 755 /etc/systemd/system/myscript.service
```
