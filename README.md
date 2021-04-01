# sample wry app

This is a WIP project. Do not use please.


### Requirements
**[wry standalone](https://github.com/lemarier/wry_standalone) is required**
To install wry standalone, follow the step bellow.

### Shell (Mac, Linux):
```bash
curl -fsSL https://raw.githubusercontent.com/lemarier/wry_standalone/main/install/install.sh | sh
```

### PowerShell (Windows):
Github require TLS 1.2 (will be removed once we use our own domain)
```bash
[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12
iwr https://raw.githubusercontent.com/lemarier/wry_standalone/main/install/install.ps1 -useb | iex
```

### Run example
```
wry run ./src/main.js
```

### Create self contained binary
For test purpose it should generate a self contained binary as `compiled-bin-test[.exe]` in the current directory.
```bash
wry compile ./src/main.js
```

#### Run the self contained binary
``` bash
./compiled-bin-test[.exe]
```