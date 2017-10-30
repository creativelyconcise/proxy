# Docker for Mac Reverse NGINX Proxy 

Stupid simple docker-compose project to get you up and running proxying URLs to your docker containers. Uses the Jwilder NGINX Proxy and Dnsmasq.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

In order to use this all you need is docker and docker-compose installed and running.

### Ready, Set, Go!

Step 1.  
Clone and run
``docker-compose up -d``

Step 2.  
Create a file at /etc/resolver/dev. Add the following

```
nameserver 127.0.0.1
port 53535
```

Yep, Really that simple. Now all requests to any domain ending in .dev will go to Docker.

## Built With

* [Jwilder NGINX Proxy](https://github.com/jwilder/nginx-proxy) - Reverse NGINX Proxy
* [Dnsmasq](https://github.com/andyshinn/docker-dnsmasq) - DNS Server


## Authors

* **Matthew Cullum** - *Initial work* - [Creatively Concise](https://github.com/creativelyconcise)


## License

This project is licensed under the MIT License
