# 401 - Class 18 Reading Notes

---

## REVIEW, RESEARCH, DISCUSSION

1. Describe a use case for a serverless function:
  - Can be cost effective. With serverless functions, you can develop any new functionality or security patch as a completely isolated, single-purpose piece of code. They decrease the possibility of downtime during a deploy. 
  - Examples: 
    - To collect, store, and dynamically display data from a DB.
    - Complete payment transactions.
    - Scale video streaming.
    - 

2. If you were to create a system that emulated Lambda functions, how would you do it?
  - I would create a websocket server with one given function, and potentially some sort of FiFo queue system to manage the requests.

3. Describe how a CDN works:
  - At its core, a CDN is a network of servers linked together with the goal of delivering content as quickly, cheaply, reliably, and securely as possible. In order to improve speed and connectivity, a CDN will place servers at the exchange points between different networks.

--- 

## Vocabulary Terms

- Serverless Functions: 
  - Serverless functions are a single-purpose, programmatic feature of serverless computing — also simply called “serverless” — a cloud computing execution model where the cloud provider provisions computing resources on demand for its customers and manages all architectures, including cloud infrastructure. 
  - [Link](https://www.splunk.com/en_us/data-insider/what-are-serverless-functions.html#:~:text=Serverless%20functions%20are%20a%20single,all%20architectures%2C%20including%20cloud%20infrastructure.)

- Cloud Storage:
  - "Cloud storage is a cloud computing model that stores data on the Internet through a cloud computing provider who manages and operates data storage as a service. It’s delivered on demand with just-in-time capacity and costs, and eliminates buying and managing your own data storage infrastructure. This gives you agility, global scale and durability, with “anytime, anywhere” data access."
  - [Link](https://aws.amazon.com/what-is-cloud-storage/)

- CDN: A content delivery network (CDN) refers to a geographically distributed group of servers which work together to provide fast delivery of Internet content.

## Links:

- [Great article for all things serverless functions](https://blog.hubspot.com/website/serverless-functions)
- [Great article on CDNs](https://www.cloudflare.com/learning/cdn/what-is-a-cdn/)
- [Great write up on Cloud Storage](https://aws.amazon.com/what-is-cloud-storage/)