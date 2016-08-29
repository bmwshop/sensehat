## Docker container for Raspberry Pi Sensehat

The goal of this project is to make the container as small as possible.  Currently, it is ~200M.

```
docker build -t sensehat .
docker run --privileged --name sensehat -ti sensehat bash
python test.py
```
Running test.py validates the installation.  See the [SenseHat API docs](https://pythonhosted.org/sense-hat/) for more SenseHat calls.

[Remon Lam's weather station docker container](https://github.com/remonlam/rpi-docker-weather/) work was really helpful in getting this to work.
