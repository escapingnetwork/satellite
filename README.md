# satellite
VSCode Remote Development Container for Urbit

This repository contains the files for running a container with Alpine Linux alongside another container with Urbit.

## Access Your Development Ship
Once the ship boot successfully access Urbit via Browser on http://localhost:81

You can see Urbit output by running:
```
$ docker logs urbit-fakezod --follow
```


### Getting and resetting the Urbit +code

This docker image includes tools for retrieving and resetting the Landscape login code belonging to the planet, for programmatic use so the container does not need a tty. These scripts can be called using docker container exec.

Getting the code:
```
$ docker container exec urbit-fakezod /bin/get-urbit-code
sampel-sampel-sampel-sampel
```

Resetting the code:
```
$ docker container exec urbit-fakezod /bin/reset-urbit-code
OK
```

Once the code has been reset the new code can be obtained from /bin/get-urbit-code.


## Start Development

To start developing mount your desk and start writing hoon!

Check the official documentation at https://developers.urbit.org/

## TODO
 - [ ] Attach VSCode terminal to Urbit container. So far Urbit crashes with STDIN on.
 - [ ] Extend README.md to explain how to add another Urbit container to test communication between ships
 - [ ] Extend README.md to explain how to boot a comet instead of fakezod
