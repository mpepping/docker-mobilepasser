# MobilePASSER in Docker

[MobilePASSER](https://github.com/datr/MobilePASSER) is a Python implementation of the MobilePASS soft-token.

## Usage


Create a `mobilepasser.cfg` configuration file with a valid activation code. An example:

```
[MobilePASS]
activation_key = QVKYC-FM6KO-SY6F7-TR22W
policy = 
index = 3
otp_length = 6
auto_update_index = True
```

Run the container:


```
docker run -ti --rm -v ${PWD}/mobilepasser.cfg:/mobilepasser.cfg mobilepasser
```
