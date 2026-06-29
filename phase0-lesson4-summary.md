# Phase 0 Lesson 4 Summary: APIs & Keys

## What This Lesson Was About

This lesson introduced the basic pattern behind API-based AI applications:

```text
send a request, get a response
```

The goal was to understand what an API is, why API keys must be protected, how
environment variables help keep keys out of code, and why beginners often use an
SDK instead of writing raw HTTP requests.

## Key Concepts

### API

API means Application Programming Interface.

Beginner-friendly meaning:

```text
An API is a doorway that lets your code use a service provided by someone else.
```

Simple analogy:

```text
Using an API is like ordering food at a restaurant.
You do not go into the kitchen yourself. You use the menu and give your order
to the service system.
```

In AI engineering:

```text
Your code sends a question to an AI provider.
The provider's servers run the model.
The API returns the model's answer.
```

This is why calling an LLM API does not require your own GPU.

### Endpoint

Beginner-friendly meaning:

```text
An endpoint is the web address where an API request is sent.
```

Example:

```text
https://api.openai.com/v1/responses
```

Simple analogy:

```text
The endpoint is like the restaurant address.
```

### API Key

Beginner-friendly meaning:

```text
An API key is a secret credential that proves who is making the request.
```

It can control:

- Who you are.
- Whether you have permission.
- Which account gets charged.

Important rule:

```text
Never write a real API key directly in code, and never upload it to GitHub.
```

### Request Body

Beginner-friendly meaning:

```text
The request body is the content you send to the API.
```

Example:

```text
Please explain neural networks in one sentence.
```

### Response Body

Beginner-friendly meaning:

```text
The response body is the result returned by the API.
```

Example:

```text
A neural network is a model that learns patterns from data through layers of
calculations.
```

### Environment Variable

Beginner-friendly meaning:

```text
An environment variable is a configuration value stored outside the code that a
program can read while running.
```

Simple analogy:

```text
The code is an employee.
The environment variable is a pass kept at the front desk.
The employee reads the pass when needed instead of carrying the secret openly.
```

In AI engineering:

```text
Put the API key in an environment variable.
Let Python read it at runtime.
Keep the real key out of the code file.
```

PowerShell example:

```powershell
$env:OPENAI_API_KEY="your-api-key"
```

Python example:

```python
import os

api_key = os.environ["OPENAI_API_KEY"]
```

### HTTP

HTTP means Hypertext Transfer Protocol.

Beginner-friendly meaning:

```text
HTTP is a set of rules computers use to send requests and responses over the
web.
```

Simple analogy:

```text
HTTP is like a delivery format. It tells the network where the package goes,
what extra information is attached, and what is inside the package.
```

An HTTP API request often includes:

- URL: where to send the request.
- Headers: extra information such as the API key.
- Body: the actual request content.

### SDK

SDK means Software Development Kit.

Beginner-friendly meaning:

```text
An SDK is a toolkit that makes it easier to use a service's API from code.
```

Simple analogy:

```text
Raw HTTP is like filling out a delivery form by hand.
An SDK is like a helper that fills out most of the form for you.
```

In AI engineering:

```text
Beginners often use an official SDK because it hides repetitive HTTP details.
The SDK usually still sends HTTP requests underneath.
```

## Exercise Answers and Feedback

### Exercise 1

Question: Identify endpoint, API key, request body, and response body.

Your answers:

```text
A. https://api.openai.com/v1/responses = endpoint
B. sk-xxxxxxxxxxxxxxxx = API key
C. Please explain neural networks in one sentence = request body
D. Neural networks are models that learn patterns from data = response body
```

Feedback:

All correct. You understood the four main parts of a basic API call.

### Exercise 2

Question: Which is safer?

Option A:

```python
api_key = "sk-real-key"
```

Option B:

```python
import os
api_key = os.environ["OPENAI_API_KEY"]
```

Your answer:

```text
B is safer, because when I upload code to GitHub, my key will not be exposed.
```

Feedback:

Correct. Environment variables help avoid the common and dangerous mistake of
putting a real key into code and pushing it to GitHub.

Important nuance:

```text
Environment variables are not magic absolute security, but they are much safer
than hardcoding secrets in code.
```

### Exercise 3

Question:

```text
1. What does HTTP do in an API call?
2. Why is an SDK easier for beginners than raw HTTP?
3. Does an SDK completely avoid HTTP underneath?
```

Status:

```text
Not answered yet.
```

This should be reviewed next time before moving deeper into hands-on API code.

## Learning Progress

Current status:

```text
Phase 0 Lesson 4: in progress
```

Understood well:

- API calls follow the request-response pattern.
- Endpoint means the API address.
- API key is a secret credential and must not be uploaded to GitHub.
- Request body is what you send.
- Response body is what you receive.
- Environment variables help keep secrets outside code.

Needs review:

- HTTP as the lower-level request-response protocol.
- SDK as a beginner-friendly wrapper around API calls.
- The relationship between SDK and HTTP.

Next step:

```text
Answer Lesson 4 Exercise 3, then continue to the first hands-on API call.
```
