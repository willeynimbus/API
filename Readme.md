# Sign Language Translation API

This is a basic backend API service for a sign language translation tool, implemented using Node.js and Express. It provides a single endpoint for translating English text input into a simulated sign language translation.

## API Endpoint

### POST /translate

Translates the provided English text into sign language (simulated).

**Request Body:**

```json
{
  "text": "Your English text here"
}
```

**Success Response:**

- **Code:** 200
- **Content:**

```json
{
  "message": "Translation successful",
  "result": "Translated: Your English text here"
}
```

**Error Response:**

- **Code:** 400
- **Content:**

```json
{
  "error": "No text provided"
}
```

## Running the Application

1. Make sure you have Node.js installed on your system.

2. Install the required dependencies:

   ```
   npm install express body-parser
   ```

3. Run the application:
   ```
   npm start
   ```

The API will be accessible at `http://localhost:3000/translate`.
