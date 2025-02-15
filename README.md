# SnapLink

SnapLink is a lightweight and efficient URL shortener built with Flask and SQLite. It allows users to shorten long URLs into compact, easily shareable links.

## Features
- Simple API for shortening and retrieving URLs
- Unique short codes generated for each URL
- Lightweight SQLite database for quick storage and retrieval
- Error handling for missing or duplicate URLs
- Easy to deploy and run locally

## Installation

### Prerequisites
- Python 3.x
- pip (Python package manager)

### Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/YOUR_USERNAME/snaplink.git
   cd snaplink
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the application:
   ```bash
   python app.py
   ```
4. The service will be available at:
   ```
   http://localhost:5000
   ```

## API Usage

### Shorten a URL
- **Endpoint:** `/shorten`
- **Method:** `POST`
- **Request Body:**
  ```json
  { "url": "https://example.com" }
  ```
- **Response:**
  ```json
  { "short_url": "http://localhost:5000/abc123" }
  ```

### Retrieve a URL
- **Endpoint:** `/{short_code}`
- **Method:** `GET`
- **Response:**
  ```json
  { "redirect_to": "https://example.com" }
  ```

## License
This project is licensed under the MIT License.

