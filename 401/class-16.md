# Serverless
Serverless is a cloud computing model that automatically provisions and scales resources to run code on demand.

AWS introduced serverless services in 2014.  Today all major cloud providers, Microsoft, Google and IBM, offer this service.

#### Serverless vs. FaaS (function as a service)

FaaS is the central element of serverless.  It provides the execution environment.  However, FaaS is a subset of serverless, which includes other anciliary services including storage, databases, networks, API gateways, and authentication.

### Serverless pros and cons

#### Pros

- Allows developers to focus on writing code for their applications, instead of managing infrastructure.
  - faster time to market
  - higher productivity
- Charges per unit of resources used.  If the application is not running, there's no charge.
  - great way to access state of the art infrastructure with a modest budget
- Enables developers to code in any language or framework -Java, python, node.js...
- Simplifies deployment and DevOps
- Provide visibility into system and user times

#### Const

- Not cost-effective with stable or predictable workloads
- Cold starts -unacceptable latancy may occur when a request follows a scale to zero event
- Monitoring and debugging are difficult to impossible using existing tools or processes
- Vendor lock-in results from deeply integrating into the specific provider environment

### Bonus: Python & APIs

> Knowing how to consume an API is one of those magical skills that, once mastered, will crack open a whole new world of possibilities, and consuming APIs using Python is a great way to learn such a skill.

To consume APIs with Python all you need is the requests library.

---

### Resources

- [Serverless](https://www.ibm.com/cloud/learn/serverless)
- [Serverless video](https://www.youtube.com/watch?v=vxJobGtqKVM)
- [Python virtual environment](https://docs.python.org/3/library/venv.html)
- [Python http.server](https://pymotw.com/3/http.server/index.html)
- [Python requests](https://docs.python-requests.org/en/latest/)
- [Python & APIs](https://realpython.com/python-api/)
- [Effective python environment](https://realpython.com/effective-python-environment/)

---

[Back to table of contents](../README.md)