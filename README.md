#eNode - A node.js eD2K/eMule Server

This is a *experimental-buggy-testing-pre-alpha* release. **Not ready to use!**

Contributions are welcome.

##Features:

* TCP/UDP opcodes
* Lugdunum/emule extended protocol
* gzip compression
* LowID Callbacks
* Files > 4GiB
* Easy support for any storage engine.
  * look at `ed2k/storage.js` and create your own `storage.<engine>.js` plugin

##Requires:

* Node.js v0.8+
* MySQL server
* Node.js modules:
  * [mysql](https://github.com/felixge/node-mysql)
  * [hexy](https://github.com/a2800276/hexy.js): to do hexdumps, useful for debugging packets
  * [tinylogger](https://github.com/petermrg/tinylogger): to show messages in console
    * [colors](https://github.com/Marak/colors.js): used in tinylogger

##Usage:

1. Create MySql database tables. Import shema in `misc/enode.sql`
2. Modify config file: `enode.config.js`
3. Execute: `node enode.js` -or- `chmod +x enode.js` and then `./enode.js`
4. You can modify the verbose level modifing the options of the `tinylogger` module

If you want to test the server on a local network, change emule options to allow local connections.

##Thanks to:

* David_X
