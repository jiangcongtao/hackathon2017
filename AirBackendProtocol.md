## Data protocol for Home IoT Controll System

* protocols: HTTP/REST
* format: json


# Endpoints

* Get current weather condition
```
HTTP Request:

http://192.168.8.112:8080/currentWeather

HTTP Response:

{"temperature":29,"unit":"C","time":"2017-03-07"}
```

* Get current control command for my device
```

HTTP Request:

http://192.168.8.112:8080/getCommand?deviceid=1


HTTP Response:

{"device":"ac-1","action":"set","newTemperature":23}
```

* Report temperator sensor data to server

```
HTTP Request:

http://192.168.8.112:8080/putWeather?temperature=39&unit=C&datetime=2017-03-05

HTTP Response:

{"okorfiail":"ok","cause":""}
```





