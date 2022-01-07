# Class 08 Reading Notes

---

## Things I want to know more about

- How often do you run into APIs that don't return JSON?

--- 

## API Design Best Practices

- [API Design Best Practices](https://gist.github.com/brookr/5977550)

### Question Answers: 

- *What does REST stand for?*
    - Representational State Transfer (REST)


- *REST APIs are designed around **resources**.*

- *What is an identifier of a resource? Give an example.*
    - "a URI that uniquely identifies that resource. "
    - Example: https://adventure-works.com/orders/1

- *What are the most common HTTP verbs?*
    - POST GET PUT DELETE

- *What should the URIs be based on?*
    - nouns

- *Give an example of a good URI.*
    - "https://adventure-works.com/orders"

- *What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?*
    - A chatty API is a web API that expose a large number of small resources.
    - It is a bad thing.
    - Should stick to "collection/item/collection"

- *What status code does a successful GET request return?*
    - 200 (OK)

- *What status code does an unsuccessful GET request return?*
    - 404 (Not Found)

- *What status code does a successful POST request return?*
    - 201 (Created)

- *What status code does a successful DELETE request return?*
    - 204 (No Content)