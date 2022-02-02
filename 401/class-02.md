# 401 - Class 02 Reading Notes

---

## REVIEW, RESEARCH, DISCUSSION

### 1. What’s the difference between PUT and PATCH?
 - PUT and PATCH are both methods for modifying some piece of data. The difference is that with PUT, the client sends the data to be modified, pre-modified. Where-as with PATCH, the client sends only the portions of the data to be modified, and a reference to piece of data to be modified, then the modification is done server-side. 

### 2. Provide links to 3 services or tools that allow you to “mock” an API for development like json-server:
  - https://mockapi.io/
  - https://www.soapui.org/learn/mocking/what-is-api-mocking/
  - https://beeceptor.com/

Compare and contrast Swagger and APIDoc.js 1 Which HTTP status codes should be sent with each type of (un)successful API call?
  - SWagger looks more like a business, where APIDoc.js looks more like an open source project.
  - APIDoc: 404
  - Swagger: 200, 400, 401, 404, 5XX
  - 
Compare and contrast SOAP and ReST
  - [Resource](https://www.redhat.com/en/topics/integration/whats-the-difference-between-soap-rest)

  - SOAP: *Simple Object Access Protocol*
    - "SOAP is a standard protocol that was first designed so that applications built with different languages and on different platforms could communicate. Because it is a protocol, it imposes built-in rules that increase its complexity and overhead, which can lead to longer page load times. However, these standards also offer built-in compliances that can make it preferable for enterprise scenarios. The built-in compliance standards include security, atomicity, consistency, isolation, and durability (ACID), which is a set of properties for ensuring reliable database transactions."

  - REST: *Representational state transfer*
    - "REST is a set of architectural principles attuned to the needs of lightweight web services and mobile applications. Because it's a set of guidelines, it leaves the implementation of these recommendations to developers."

  > REST and SOAP are 2 different approaches to online data transmission. Specifically, both define how to build application programming interfaces (APIs), which allow data to be communicated between web applications. Representational state transfer (REST) is a set of architectural principles. Simple object access protocol (SOAP) is an official protocol maintained by the World Wide Web Consortium (W3C). The main difference is that SOAP is a protocol while REST is not. Typically, an API will adhere to either REST or SOAP, depending on the use case and preferences of the developer.

- SOAP vs REST: 
  - "Many legacy systems may still adhere to SOAP, while REST came later and is often viewed as a faster alternative in web-based scenarios. REST is a set of guidelines that offers flexible implementation, whereas SOAP is a protocol with specific requirements like XML messaging.

REST APIs are lightweight, making them ideal for newer contexts like the Internet of Things (IoT), mobile application development, and serverless computing. SOAP web services offer built-in security and transaction compliance that align with many enterprise needs, but that also makes them heavier. Additionally, many public APIs, like the Google Maps API, follow the REST guidelines."

## Vocabulary Terms

- Web Server:
  - "On the hardware side, a web server is a computer that stores web server software and a website's component files. (for example, HTML documents, images, CSS stylesheets, and JavaScript files) A web server connects to the Internet and supports physical data interchange with other devices connected to the web." - Mozilla
  
- Express: 
  - A web server software, it is a framework that runs on Node.js and facilitates HTTP requests for web and mobile applications.

- Routing:
  - Routing is a process that is performed by layer 3 (or network layer) devices in order to deliver the packet by choosing an optimal path from one network to another. 
    - There are 3 types of routing: 
      - Static
      - Default
      - Dynamic

- WRRC:
  - WRRC stands for Web Request Response Cycle, and it documents or models the flow or exchange of data between client and server. 

## Preview: 

1. Which 3 things had you heard about previously and now have better clarity on?
   - Middleware
   - Modules
   - Managing complexity in large code bases.
2. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
   - I am hoping to combined my knowledge of the three things previously mentioned with:
     - APIs
     - Authorization
     - Client Side Applications 
3. What are you most excited about trying to implement or see how it works?
   - I'm not sure that I am excited about it, because it is always complicated, but I'm interested to hear more about how we keep our code bases secure.