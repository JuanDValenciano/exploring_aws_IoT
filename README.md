# exploring_aws_IoT
My study notes from the course: https://www.udemy.com/course/exploring-aws-iot

## Getting setup

To use the Sketch with the ESP8266 board

- Arduino IDE 1.8.19
- ESP8266 Community Version 2.7.4 [https://github.com/esp8266/Arduino/tree/2.7.4]
- PubSubClient Version 2.8.0 [https://github.com/knolleary/pubsubclient/tree/v2.8]

Python files haven't dependencies. use a 3.4+ version.

### ESP8266

For each Sketch you must configure the WiFi credentials:

```
const char* ssid = "<YOUR-WIFI-NETWORK>";
const char* password = "<YOUR-WIFI-PASSWORD>";
```

the EndPoint:

```
const char* awsEndpoint = "YOUR-ACCOUNT-ID-ats.iot.YOUR-CERTIFICATE-REGION.amazonaws.com";
```

and the certificates:

```
certificate.pem.crt
private.pem.key
```

all this data must be confirmed on the AWS IoT platform

### Python

To use the python script you just need to add the data, example:

```
$python main.py --endpoint YOUR-ACCOUNT-ID-ats.iot.YOUR-CERTIFICATE-REGION.amazonaws.com --cert ../certificate.pem.crt --key ../private.pem.key --topic outTopi
```

### Bash

....

## Project Base

- [AWS-IoT](https://github.com/sborsay/AWS-IoT)