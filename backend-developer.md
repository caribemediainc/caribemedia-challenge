# Backend Developer Challenge

The assignment is designed to check your coding and problem-solving skills. Use modern tools and practices. We suggest you spend a maximum of 8-12 hours on it.

**Things we require your code to have:**

- **Domain Model Design**: Implement DDD concepts: aggregates, value objects, domain services, etc.
- **Messaging System (optional)**: Implement Queues, Events, Commands.
- **Code Organization**: Ensure modularity and proper dependencies.
- **Exception Handling and Logging**: Robust error management and informative logging.
- **Testing**: Comprehensive test suite covering key functionalities.
- **Asynchronous Programming**: Efficient task-based asynchronous patterns.
- **Deployment Process**: Documented and reproducible deployment steps.

**Note**: No UI needed.

## Requirements

#### Auth Module

- Generate a token for valid email/password combinations.
- Return "Oops! wrong password" for invalid credentials.
- Send a welcome email on new user registration.

#### Listing Module

- The user can search for a business using a term.
- The user can list all available listings depending on its city.
- The user can sort the listings by all the available params.

Listing shape example:

```json
[
  {
    "name": "Consolidated Moving & Storage SRL",
    "description": "39 Years of Professional Moving Services Packing Moving Storage Local & Long Distance Fully Licensed & Insured WSIB Certified Guaranteed Competitive Quotations",
    "country": "Dominican Republic",
    "city": "Santo Domingo",
    "zip_code": 10123,
    "address": "542 Mount Pleasant Santo Domingo",
    "phone": "+1 (809) 654-0983",
    "tags": ["services", "storage", "movements"],
    "website": "https://www.consolidatedmoving.com.do",
    "categories": [{ "id": 1, "name": "Movements", "points": 2 }],
    "payment_methods": [
      { "id": 1, "name": "Visa" },
      { "id": 1, "name": "Mastercard" }
    ],
    "schedule": [
      { "id": 100, "day": 1, "open": "7:00", "close": "18:00" },
      { "id": 101, "day": 2, "open": "7:00", "close": "18:00" },
      { "id": 102, "day": 3, "open": "7:00", "close": "18:00" },
      { "id": 103, "day": 4, "open": "7:00", "close": "18:00" },
      { "id": 104, "day": 5, "open": "7:00", "close": "18:00" }
    ],
    "languages": [{ "id": 1, "language": "spanish" }],
    "logo": "https://picsum.photos/200/300"
  },
  {
    "name": "Affordable Movers and Packers INC",
    "description": "Looking for trust worthy and efficient service from local movers? You won’t be disappointed by our team of Affordable Movers! With the help of our professional movers, you will be ensured of an efficient relocation.",
    "country": "Dominican Republic",
    "city": "Santiago",
    "zip_code": 34123,
    "address": "23 John St Rd, Santiago",
    "phone": "+1 (849) 546-1334",
    "tags": ["movement", "storage", "packs"],
    "website": "https://www.affordabledo.com.do",
    "categories": [
      { "id": 1, "name": "Movements", "points": 7 },
      { "id": 7, "name": "Packing", "points": 2 }
    ],
    "payment_methods": [
      { "id": 1, "name": "Visa" },
      { "id": 1, "name": "Mastercard" },
      { "id": 1, "name": "American Express" }
    ],
    "schedule": [
      { "id": 100, "day": 1, "open": "9:00", "close": "13:00" },
      { "id": 101, "day": 2, "open": "9:00", "close": "13:00" },
      { "id": 102, "day": 3, "open": "9:00", "close": "13:00" },
      { "id": 103, "day": 4, "open": "9:00", "close": "13:00" },
      { "id": 104, "day": 5, "open": "9:00", "close": "13:00" }
    ],
    "languages": [{ "id": 1, "language": "english" }],
    "logo": "https://picsum.photos/200/300"
  }
]
```

## Deliverables

1. Use **REST** to build the API
2. **Language**: Typescript.
3. **Backend Framework**: Choose one - Nest.js (desirable), Express.js, or Fastify.
4. **Database**: Any, with a preference for Postgres or NoSQL CosmosDB.
5. **Cloud Deployment**: Azure preferred. Provide access to a working API instance.
6. **CI/CD**: Setup a continuous integration server for tests and deployment (e.g., GitHub Actions).

## Nice to have (not required)

1. **Search Engine Integration**: Elastic Search or Azure Cognitive Search.
2. **Serverless Functions**: Utilize Azure Functions.
3. **GitHub Actions**: For Dockerization and deployment.
4. **Containerization and Orchestration**: Dockerize your application and prepare it for Kubernetes deployment.

**Note:** Ensure your code is efficient, readable, and well-documented. Good luck.
