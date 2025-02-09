# **Quotes-API Documentation**

## **Introduction**
Quotes-API provides a collection of inspiring, motivational, and thought-provoking quotes categorized by type and author. This API allows developers to integrate quotes into applications, websites, or personal projects seamlessly.

---

## **Base URL**
```
https://quotes-api12.p.rapidapi.com
```

---

## **Authentication**
To use Quotes-API, you need an API key from **RapidAPI**.
- Sign up on RapidAPI.
- Subscribe to Quotes-API.
- Use the provided API key in your requests.

**Headers:**
```
X-RapidAPI-Key: YOUR_API_KEY
X-RapidAPI-Host: quotes-api.rapidapi.com
```

---

## **API Endpoints**

### **1. Fetch a Random Quote**
Retrieve a random quote from the database.

**Endpoint:**
```
GET /quotes
```
**Response:**
```json
{
  "quote": "Success is about doing what you love and being happy doing it.",
  "author": "Unknown",
  "type": "success"
}
```

---

### **2. Fetch All Quote Categories**
Retrieve a list of all available quote types.

**Endpoint:**
```
GET /type
```
**Response:**
```json
{
  "length": 3,
  "types": ["success",
            "inspirational", 
            "self-confidence"
    ]
}
```

---

### **3. Fetch All Authors**
Retrieve a list of all authors along with their quote count.

**Endpoint:**
```
GET /author
```
**Response:**
```json
{
  "length": 3,
  "authors": [
    "Unknown", 
   "Brian Tracy", 
   "Winston Churchill"
  ]
}
```

---

### **4. Fetch Quotes by Type**
Retrieve all quotes belonging to a specific category.

**Endpoint:**
```
GET /quotes/random?type={type}
```
**Example:**
```
GET /quotes/random?typesuccess
```
**Response:**
```json
{
  "quote": "Success is about doing what you love.",
  "author": "Unknown", 
  "type": "success"
}
```

---

### **5. Fetch Quotes by Author**
Retrieve all quotes from a specific author.

**Endpoint:**
```
GET /quotes/author/{author_name}
```
**Example:**
```
GET /quotes/author/Steve%20Jobs
```
**Response:**
```json
{
  "length": 2,
  "quotes": [
    {"quote": "Innovation distinguishes between a leader and a follower.", 
     "author": "Steve Jobs"
    },
    {"quote": "Your time is limited, don’t waste it living someone else’s life.",
     "author": "Steve Jobs"
    }
  ]
}
```

---

## **Rate Limits**
Quotes-API enforces rate limits as specified on **RapidAPI**. Exceeding these limits may lead to temporary suspension.

---

## **Terms of Use**
By using Quotes-API, you agree to:
- Use the API for personal, educational, or non-commercial purposes.
- Not sell, reproduce, or redistribute API data without permission.
- Comply with RapidAPI’s terms and conditions.

---

## **Contact Information**
For support or inquiries, contact us at **shreekant4062@gmail.com**.

**Start integrating Quotes-API today and bring daily inspiration to your users! 🚀**

