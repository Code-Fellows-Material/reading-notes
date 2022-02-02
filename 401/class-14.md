# 401 - Class 14 Reading Notes

---

## REVIEW, RESEARCH, DISCUSSION

1. What’s the difference between a FIFO and a standard queue?
    - FiFo hold the messages in the order they were received, standard queues only hold a reference to all messages by name/id/some defined property.

2. How can the server be assured a message was properly received?
    - By creating some sort of expected communication of receipt. 

3. What classic design pattern is best represented by event driven programming?
    - Pub/Sub

4. How do you test an event driven system?
    - Logging and in more advanced systems automation.

--- 

## Vocabulary Terms

  - FIFO Queue: A FIFO queue is an ordered list of elements where an element is inserted at the end of the queue and is removed from the front of the queue.

[FIFO Queue](https://www.javascripttutorial.net/javascript-queue/)

  - Pub/Sub: The Publish/Subscribe pattern, also known as pub/sub, is an architectural design pattern that provides a framework for exchanging messages between publishers and subscribers. This pattern involves the publisher and the subscriber relying on a message broker that relays messages from the publisher to the subscribers.

[FPub/Sub](https://aws.amazon.com/pub-sub-messaging/)