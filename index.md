# Personal projects

In this page you will find a link to all my open source personal projects. They were created to fill a need that I had at the moment and could not find any existing solution out there. Some of them are abandoned, as there's no need to use them anymore.

### Cachet URL monitor ![GitHub stars](https://img.shields.io/github/stars/mtakaki/cachet-url-monitor.svg?style=flat-square)![GitHub](https://img.shields.io/github/license/mtakaki/cachet-url-monitor.svg?style=flat-square)
This tool monitors a given set of URLs and verifies its state, including regex matching against the response body, HTTP status, and response latency. It's meant to be used along [CachetHQ](http://cachethq.io/), which is an awesome status page.

This project is fully written in Python and it's better used with docker.

[https://github.com/mtakaki/cachet-url-monitor](https://github.com/mtakaki/cachet-url-monitor)

### Dropwizard circuit breaker ![GitHub stars](https://img.shields.io/github/stars/mtakaki/dropwizard-circuitbreaker.svg?style=flat-square)![GitHub](https://img.shields.io/github/license/mtakaki/dropwizard-circuitbreaker.svg?style=flat-square)
This is a plugin for dropwizard, that can also be used standalone, and it provides circuit-breaking functionality to your web service. It will automatically measure the rate of failures and open the circuit when it reaches a configured threshold. It differs from tenacity by being a simpler implementation, not having a distributed metric aggregation. It will only measure the rate on one instance.

[https://github.com/mtakaki/dropwizard-circuitbreaker](https://github.com/mtakaki/dropwizard-circuitbreaker)

### Dropwizard HikariCP ![GitHub stars](https://img.shields.io/github/stars/mtakaki/dropwizard-hikaricp.svg?style=flat-square)![GitHub](https://img.shields.io/github/license/mtakaki/dropwizard-hikaricp.svg?style=flat-square)
Provides a dropwizard bundle that allows you to use [HikariCP](https://github.com/brettwooldridge/HikariCP) as the database connection pool, replacing the default Tomcat connection pool. The README provides some benchmarking comparison, but there are more comprehensive literature out there (please see the link in the README). It was created to provide an alternative to dropwizard's default bundle.

[https://github.com/mtakaki/dropwizard-hikaricp](https://github.com/mtakaki/dropwizard-hikaricp)

### Dropwizard admin resource ![GitHub stars](https://img.shields.io/github/stars/mtakaki/dropwizard-admin-resource.svg?style=flat-square)![GitHub](https://img.shields.io/github/license/mtakaki/dropwizard-admin-resource.svg?style=flat-square)
Another dropwizard bundle that allows you to easily register resources under the admin port. This provides you a way to create internal APIs, as your admin port should not be publicly exposed, without having to go through the whole hassle of figuring out the internal parts of dropwizard.

[https://github.com/mtakaki/dropwizard-admin-resource](https://github.com/mtakaki/dropwizard-admin-resource)

### Dropwizard Jodd Petite bundle ![GitHub stars](https://img.shields.io/github/stars/mtakaki/dropwizard-petite.svg?style=flat-square)![GitHub](https://img.shields.io/github/license/mtakaki/dropwizard-petite.svg?style=flat-square)
Another dropwizard bundle that integrates [Jodd Petite](https://jodd.org/petite/), providing a extremely simple and lightweight dependency injection tool. The idea was to steer away from the industry standard Spring, which is sometimes an overkill for many microservices.

[https://github.com/mtakaki/dropwizard-petite](https://github.com/mtakaki/dropwizard-petite)

### Credential storage service ![GitHub stars](https://img.shields.io/github/stars/mtakaki/CredentialStorageService.svg?style=flat-square)![GitHub](https://img.shields.io/github/license/mtakaki/CredentialStorageService.svg?style=flat-square)
Pet project from this idea of having a better way to store credentials and secrets, without having to store them in plain-text configuration files. This only works well when used with the [dropwizard hibernate bundle](https://github.com/mtakaki/CredentialStorageService-dw-hibernate). The idea is to not require providing the username and password in your configuration YAML file and it will automatically fetch the credentials from the server (which are fully encrypted) and, instead, it uses a public and private key. It also provides the ability to poll for changes and it automatically rotates the connection pool from one credential to another, all done gracefully and without dropping any requests.

[https://github.com/mtakaki/CredentialStorageService](https://github.com/mtakaki/CredentialStorageService)

### Dropwizard hibernate test utility ![GitHub stars](https://img.shields.io/github/stars/mtakaki/dropwizard-hibernate-test-util.svg?style=flat-square)![GitHub](https://img.shields.io/github/license/mtakaki/dropwizard-hibernate-test-util.svg?style=flat-square)
Provides a JUnit test rule for testing hibernate DAOs, spawning an in-memory database for integration tests. It simplifies the need to write your own test harness for every unit test.

[https://github.com/mtakaki/dropwizard-hibernate-test-util](https://github.com/mtakaki/dropwizard-hibernate-test-util)

### Dropwizard logentries appender (abandoned) ![GitHub stars](https://img.shields.io/github/stars/mtakaki/dropwizard-logentries-appender.svg?style=flat-square)![GitHub](https://img.shields.io/github/license/mtakaki/dropwizard-logentries-appender.svg?style=flat-square)
Dropwizard log appendar that integrates with [logentries](https://logentries.com/). It provides and out-of-the-box integration and simple configuration.
This project has not been kept up to date, as I don't use logentries anymore.

[https://github.com/mtakaki/dropwizard-logentries-appender](https://github.com/mtakaki/dropwizard-logentries-appender)
