## Standard for strucutred logs

### Problem

### Solution




niquola notes:

>   ### Problem
>
>   * combinatorial explosure in logging & monitoring
>   * microservices - tracing
>   * metrics, errors & logs are related
>
>   ### Solution
>
>   Create standard format for structured logs
>
>   ### Key Points
>
>   * JSON storages frendly - no name clashes
>   * OpenTracing.io frendly - spans
>   * syslog fields
>   * elk fields
>   * distributed system (node, application, module, id, geoIp, etc)
>   * metrics frendly (prometheus, collectd)
>   * JSON schemata - published into one repo
>   * application logging libraries
>   * file system as buffer 
>   * go library to simplify aggregation & routing


### Classical log levels

* log levels: DEBUG, INFO etc 

### log4j

https://logging.apache.org/log4j/1.2/apidocs/org/apache/log4j/PatternLayout.html

* category "a.b.c"
* file name
* location - domain name
* line number
* message
* method-name
* priority
* thread-name
* nested context

### Log back

https://logback.qos.ch/manual/layouts.html

### ELK

* @timestamp - timestamp field  (http://dev.haufe.com/log-aggregation/)


### Network

* ip
* dns

### Syslog

https://en.wikipedia.org/wiki/Syslog

* severity level
* facility
* message


