# CT_subdomains
An hourly updated list of subdomains gathered from certificate transparency logs. 

## How it works
We use [certstream](https://github.com/CaliDog/certstream-python/) to subscribe to the certificate transparency log stream. When an update is broadcasted, the domain is parsed and all subdomains inserted into our database.

A second script exports the top 100/1000/10,000/100,000 observered subdomains and pushes them into this repository on an hourly basis.

