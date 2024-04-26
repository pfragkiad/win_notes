# win_notes

## Show wlans

To show all wlan profiles:

```cmd
netsh wlan show profile
```

To show full profile information (e.g for the profile "keftes") including the key:

```cmd
netsh wlan show profile name="keftes" key=clear
```

To show just the key we can filter out just the field:

```cmd
netsh wlan show profile name="keftes" key=clear | findstr "Key Content"
```
