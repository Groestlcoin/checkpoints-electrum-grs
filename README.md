# checkpoints-electrum-grs

This tool is written to generate the checkpoints.json file which is used in Electrum-GRS for Groestlcoin.

A checkpoints.json file can be found in electrum-grs clients.

##### Minimum Recommended Specifications

- **Go 1.10 or 1.11**
* Linux


  Installation instructions can be found here: https://golang.org/doc/install.
  It is recommended to add `$GOPATH/bin` to your `PATH` at this point.

#### setup
``cd ~/go/src/github.com/``

``git clone https://github.com/groestlcoin/checkpoints-electrum-grs.git``

``cd checkpoints-electrum-grs``

``dep ensure``


dep is a dependency management tool for Go. It requires Go 1.9 or newer to compile.
https://github.com/golang/dep

### config.yml

change the host, port, username & password so it matches your RPC credentials.

### Running the app

You can run the app by using the following command:

``go run main.go``

Or you can build the binary with the following command

``go build main.go``

This will produce a binary called "main" wich you can rename and for example upload
on the server with scp as example. With the compiled binary, your linux
server/vps does not need the dependency's. The server/VPS that will run the binary
does not need to have Golang installed at all.

The machine that will compile does need Golang installed and all dependency's (use dep).

License
-------

This tool is released under the terms of the MIT license. See [COPYING](COPYING) for more
information or see https://opensource.org/licenses/MIT.
