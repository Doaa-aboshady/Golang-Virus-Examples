## Golang Virus Examples

### Malware

#### ExfilDocs
* Searches drive for specific file extensions
* Uploads files to C2 via SSH
 

#### Outlook Exfil
* Asks for Outlook Credentials
* Authenticates via IMAP, searches attachments and uploads files to C2 via SSH
TO DO: Fix Windows Compilation


#### Screen Shotter
* Uploads screenshot every 20 seconds to C2 via SSH

#### Dropper 
* Hosts 3 files, downloads them from itself then executes them.


Compile to windows:
CGO_ENABLED=1 CC=/usr/local/Cellar/mingw-w64/5.0.4_1/bin/x86_64-w64-mingw32-gcc CXX=/usr/local/Cellar/mingw-w64/5.0.4_1/bin/x86_64-w64-mingw32-g++ GOOS=windows GOARCH=amd64 go build .
