# satellite
VSCode Remote Development Container for [Urbit](urbit.org/)

This repository include the files for running a container with

- Urbit CLI
- [Bouncer](https://github.com/tloncorp/bouncer)
- [Hoon Language Server](https://github.com/urbit/hoon-language-server)
- [Hoon Language Support](https://marketplace.visualstudio.com/items?itemName=tloncorp.hoon-tloncorp)
- [Hoon Assist](https://marketplace.visualstudio.com/items?itemName=nocsyx-lassul.hoon-assist)

## Requeriments

- [Visual Studio Code](https://code.visualstudio.com/)
- [Docker](https://www.docker.com/)
- [VSCode - Remote Development Extension](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.vscode-remote-extensionpack)

For more information about developing inside a Container [check this documentation](https://code.visualstudio.com/docs/remote/containers).

## Access Your Development Ship
Once VSCode is attached to the running container it will start Urbit Fakezod, access Urbit via Browser on http://localhost:81


### Getting Urbit +code

Get the code writting the following command on the VSCode terminal runninng Urbit:
```
+code
```

### Start Urbit Language Server
```
|start %language-server
```

## Start Development

To start developing mount your desk and start writing hoon!

Check the official documentation at https://developers.urbit.org/