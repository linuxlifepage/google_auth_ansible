## 2FA GOOGLE FOR SSH

### Для повторного запуска ansible необходимо либо скопировать команду и запустить ее вручную. Либо добавить в исключение IP в конфиг ssh с которого запускается ansible

```
Match Address 192.168.1.0/24 # Или же конкретный IP 192.168.1.15
    AuthenticationMethods publickey keyboard-interactive
```
