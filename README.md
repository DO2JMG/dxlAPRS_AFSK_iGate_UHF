dxlAPRS Internet Gateway for raspberry pi

### Unpack  :

```
  git clone https://github.com/DO2JMG/dxlAPRS_AFSK_iGate_UHF.git
  cd dxlAPRS_AFSK_iGate_UHF
```

### Create folders and permissions  :

```
  mkdir bin
  mkdir fifos
  mkdir pidfiles
```
```
  sudo chmod +x afsk.sh
```

### Download dxlAPRS  :

```
  cd bin
  wget http://oe5dxl.hamspirit.at:8025/aprs/bin/armv7hf/afskmodem
  wget http://oe5dxl.hamspirit.at:8025/aprs/bin/armv7hf/udpgate4
  wget http://oe5dxl.hamspirit.at:8025/aprs/bin/armv7hf/sdrtst
```

Permissions

```
  cd bin
  sudo chmod +x afskmodem
  sudo chmod +x udpgate4
  sudo chmod +x sdrtst
```
```
  cd ..
```
### Settings  :
  Change your call and passcode in options.conf

```
  nano options.conf
```

  Change your beacon message in beacon.txt
```
  nano beacon.txt
```
  
### Run  :

Start

  ```
    ./afsk.sh
  ```
Stop

  ```
  ./afsk.sh stop
  ```
