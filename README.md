# TASK-1
Guvi Zen class Elakkiya's TASK 1
## 1. Write a blog on Difference between HTTP1.1 vs HTTP2

### Evolution: HTTP
HTTP, the protocol that powers the web, has seen a significant evolution over the years. The transition from HTTP/1.1 to HTTP/2 brought about fundamental changes, enhancing performance, security, and efficiency. Let's dive into the key differences between the two versions.

### HTTP 1.1:
1. Serial Processing:
Limitation: HTTP/1.1 operates with a single request-response mechanism at a time. This serial processing leads to inefficiencies, especially on high-latency connections.
2. Header Redundancy:
Issue: With every request, headers are present, causing redundant data transmission and consuming bandwidth unnecessarily.
3. Resource Bundling:
Drawback: Bundling multiple resources (like CSS, JavaScript, etc.) into one file is common. However, if even a single resource is needed, the entire bundle has to be downloaded.
4. No Multiplexing:
Challenge: Lacks the ability to multiplex multiple requests simultaneously over a single TCP connection, resulting in slower page loads.

### HTTP2 :
1. Multiplexing:
Improvement: Introduces multiplexing, enabling multiple requests and responses concurrently within a single TCP connection. This significantly reduces latency and speeds up page loading times.
2. Header Compression:
Optimization: Headers are compressed, decreasing overhead and reducing redundant data transmission, thereby conserving bandwidth.
3. Server Push:
Advantage: Allows servers to push multiple responses proactively to the client, eliminating the need for additional round trips to request necessary resources.
4. Binary Protocol:
Enhancement: HTTP 2 uses a binary protocol instead of plain text, making it more efficient for parsing and reducing errors.
5. Stream Prioritization:
Feature: Prioritises critical resources, ensuring important assets are delivered first, optimising page rendering.

### Conclusion:
The shift from HTTP1.1 to HTTP2 marks a significant advancement in web protocol technology. HTTP2's multiplexing, header compression, and other enhancements have revolutionised web performance, resulting in faster, more efficient, and secure web experiences.Adopting HTTP/2 offers substantial advantages over its predecessor, contributing to a faster, smoother, and more responsive web, benefitting both users and businesses alike.

## Write a blog about objects and its internal representation in Javascript

Exploring Objects and Their Internal Representation in JavaScript. JavaScript, as an object-oriented language, revolves around the concept of objects. These objects serve as the building blocks for creating complex data structures, and understanding their internal representation is crucial for effective programming.

### Objects in JavaScript:
1. Object Creation:
In JavaScript, objects are collections of key-value pairs. They can be created using various methods:
Literal Notation: const obj = { key: value };
Constructor Notation: const obj = new Object(); obj.key = value;

2. Properties and Methods:
Properties: Represent characteristics of an object, stored as key-value pairs.
Methods: Functions defined within an object, allowing the object to perform actions.

3. Dynamic Nature:
JavaScript objects are mutable, allowing properties to be added, modified, or deleted dynamically.

### Internal Representation:
1. Memory Allocation:
Objects in JavaScript are stored in memory as references. When you create an object, a reference to it is stored in memory, pointing to its actual location.

2. Properties and Prototypes:
Each object has a prototype (except for the base object) which it inherits properties and methods from.
Properties and methods are stored in a hashmap-like structure, allowing quick access based on the property name.

3. Primitive vs. Reference Types:
Primitive types (like strings, numbers, etc.) are stored directly in memory, while objects (reference types) hold a reference to the memory location where their data is stored.

4. Copy by Reference:
When assigning an object to another variable, it's the reference that's copied, not the object itself. Modifications to one reference will affect the other since they point to the same object.


EXAMPLE: 

const car = {
    brand: 'Tesla',
    model: 'Model S',
    year: 2023
};

const carReference = car; // Both 'car' and 'carReference' point to the same object

carReference.year = 2024;
console.log(car.year); // Output: 2024 (since both variables reference the same object)

Understanding how JavaScript handles objects internally is essential for writing efficient and maintainable code. Manipulating objects, considering their references, and utilizing their dynamic nature can lead to powerful and flexible solutions in JavaScript programming.

Objects form a cornerstone in JavaScript, offering a versatile and dynamic way to structure and manage data within the language.

