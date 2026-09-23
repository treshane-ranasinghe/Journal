Learning Journal Day 0

Name: Treshane Ranasinghe

1. What I Already Know

I know that a client sends an HTTP request to an API endpoint, and that the server processes it and returns a status code and a response body. What I don't know yet: how production APIs keep responses consistent across every endpoint.

I know path parameters identify a specific resource (/users/42) and query parameters filter or sort a collection (/users?role=admin). What I don't know yet: where to draw the line in less obvious cases, such as search, nested resources (/users/42/orders), or optional filters.

 I can send and receive JSON request and response bodies, and I know headers carry metadata such as Content-Type and Authorization. What I don't know yet: a clear rule for when data belongs in a header rather than in the body or the URL.

2. What I Want to Understand by Day 5

API structure: - I can build REST APIs, but I don't fully understand how to design one well. By Day 5, I want to take one of my own APIs, list its resources and endpoints, and explain why each endpoint is structured that way.

Where data goes: -  I know JSON bodies, query parameters, path parameters, and headers, but I'm not always sure which one to use. By Day 5, I want to look at the requests in my own API and say where each piece of data belongs and why.

Consistent/ maintainable APIs: -  By Day 5, I want to explain the basic principles of a consistent, easy-to-maintain API and use them to fix at least one inconsistency in my own project.

3. My Learning Style

Hands-on practice with projects and repetitive studying. I understand a concept properly once I build something with it, like an API endpoint in FastAPI, and test it myself. Going over the same topic several times helps it stick, and practical work shows me the gaps that reading alone would miss.

I search on Google and use AI tools to stay efficient and productive. This helps me find answers and examples quickly and keeps my work moving. The downside is that I sometimes get a working solution without fully understanding why it works.

When I get stuck, spend 1 hour trying to solve it myself before using Google or AI. During that hour I will read the error messages, check my code step by step, and write down what I think is going wrong. After I find the answer, I will write a short note in my own words explaining why it works, so I learn the concept instead of just fixing the problem.