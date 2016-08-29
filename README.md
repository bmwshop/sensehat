## Docker container for Raspberry Pi Sensehat

The goal of this project is to make the container as small as possible.  Currently, it is ~200M.

'''
docker build -t sensehat .
docker run --privileged --name sensehat -ti sensehat bash
```
The test.py is a starting point, see the [SenseHat API docs](https://pythonhosted.org/sense-hat/) for more.

[Remon Lam's weather station docker container](https://github.com/remonlam/rpi-docker-weather/) work was really helpful in getting this to work.
