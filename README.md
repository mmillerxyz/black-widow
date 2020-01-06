# Black Widow

[![Python 3.x](https://img.shields.io/badge/python-3.x-yellow.svg)](https://www.python.org/) [![License](https://img.shields.io/badge/license-GPLv3-red.svg)](https://raw.githubusercontent.com/FabrizioFubelli/black-widow/master/LICENSE) [![Docker Pulls](https://img.shields.io/docker/pulls/offensive/black-widow.svg)](https://hub.docker.com/r/offensive/black-widow) 

![image](https://raw.githubusercontent.com/offensive-hub/black-widow/master/resources/black-widow-img.png)

## Offensive penetration testing tool \(Open Source\)

**black-widow** is one of the most useful, powerful and complete offensive penetration testing tool.

It provides easy ways to execute many kinds of information gatherings and attacks.

* Fully Open Source
* Written in Python
* Continuously updated and extended

### Features:

* [x] Localhost Web GUI
* [x] Sniffing
* [x] Website crawling
* [x] Web page parsing
* [ ] SQL injection
* [ ] Injected database management
* [ ] Brute force attacks
* [ ] Cluster between other black-widows
* [ ] Multiple asynchronous requests
* [ ] Multiple targets management
* [ ] Useful CTF features

### ![DOCKER\_IMAGE](https://docs.docker.com/favicons/docs@2x.ico) Docker Installation:

1. If you haven't Docker, [install it](https://docs.docker.com/install/linux/docker-ce/ubuntu)
2. Run docker:
   * Command line: `docker run --rm offensive/black-widow [arguments]`
   * GUI: `docker run -d -p 8095:80 --rm offensive/black-widow -g`
     * Than visit: [http://localhost:8095](http://localhost:8095/)

### Default Installation:

1. `sudo apt-get update && sudo apt-get install tidy clang tshark`
2. `git clone git@github.com:offensive-hub/black-widow.git`
3. `cd black-widow`
4. `sudo pip3 install -U -r requirements.txt`
5. `sudo ./black-widow.py --django migrate`
6. `sudo ./black-widow.py <arguments>`

### Run:

* **GUI:** `sudo ./black-widow.py -g`
* **Command line:** `sudo ./black-widow.py <arguments>`

### Debug:

* Run django \(examples\):
  * `./black-widow.py --django runserver`
  * `./black-widow.py --django help`
  * `./black-widow.py --django "help createsuperuser"`

### Directories:

```text
TODO: fix the following directory tree
[root]
  |
  |-- app/      # Main application package
  |    |
  |    |-- attack/         # Package per modalità di attacco
  |    |-- defense/        # Package per modalità di difesa
  |    |
  |    |-- gui/            # Package per la grafica dell'applicazione
  |    |
  |    |-- storage/        # Package per salvare i files (settings, output, ...)
  |    |
  |    |-- utils/
  |    |    |
  |    |    |-- cluster/        # Package che fornisce metodi per condividere e ricevere info
  |    |    |-- crypto/         # Package per criptare/decriptare/codificare/decodificare stringhe e files
  |    |    |-- exceptions/     # Eventuali eccezioni personalizzate
  |    |    |-- helpers/        # Package contenente helpers generici usati in più parti del programma
  |    |    |-- history/        # Package che fornisce classi e funzioni per salvare cronologie di vario tipo
  |    |    |-- html/           # Package che fornisce metodi per fare il parsing di un html
  |    |    |-- requests/       # Package che fornisce metodi per effettuare richieste (anche multiple)
  |    |    |-- settings/       # Package dedito al settaggio di parametri globali (es. IP gaming server, ...)
  |    |    |-- sniffing/       # Package che fornisce metodi per sniffing in una rete
  |    |    |-- sql/            # Package che fornisce metodi per sql injection
  |    |
  |    |-- env.py          # Variabili d'ambiente
  |
  |-- black-widow.py   # Eseguibile principale
  |-- test.py          # Eseguibile di testing
```

### Links:

* Homepage: [https://black-widow.io](https://black-widow.io)
* GitHub: [https://github.com/offensive-hub/black-widow](https://github.com/offensive-hub/black-widow)
* Docker Registry: [https://hub.docker.com/r/offensive/black-widow](https://hub.docker.com/r/offensive/black-widow)
* Free Software Directory: [https://directory.fsf.org/wiki/Black-widow](https://directory.fsf.org/wiki/black-widow)

### Contacts:

* [offensive-hub@protonmail.com](mailto:offensive-hub@protonmail.com)

### Authors:

* [Fabrizio Fubelli](https://fabrizio.fubelli.org)

### Thanks to:

* [PyShark](https://github.com/KimiNewt/pyshark)
* [Sqlmap](https://github.com/sqlmapproject/sqlmap)
* [Material Dashboard](https://github.com/creativetimofficial/material-dashboard)

### Follow Us:

