# sample wry app

This is a WIP project. Do not use please.


### Requirements
**[wry standalone](https://github.com/lemarier/wry_standalone) is required** follow the step below.

You should only install wry once. We will probably also push binary via a deno script or a node package.

#### Shell (Mac, Linux):
```bash
curl -fsSL https://raw.githubusercontent.com/lemarier/wry_standalone/main/install/install.sh | sh
```

#### PowerShell (Windows):
Github require TLS 1.2 (will be removed once we use our own domain)
```bash
[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12
iwr https://raw.githubusercontent.com/lemarier/wry_standalone/main/install/install.ps1 -useb | iex
```

### Run example
```bash
git clone https://github.com/lemarier/wry_demo.git
cd wry_demo
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