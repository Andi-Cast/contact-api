# Contact API

## Overview
This Contact API provides a comprehensive backend service for managing contact information. With this API, you can create, retrieve, update, and delete contact records, as well as upload and retrieve contact photos. The API supports pagination for listing contacts and is designed to handle image uploads efficiently.

## Application Details
The Contact API allows users to manage their contact information including name, email, phone, address, title, status, and photo. It provides endpoints for CRUD operations on contacts, photo management, and pagination of contact lists.

## Features
- Create, read, update, and delete contact records
- Upload and retrieve contact photos
- Pagination for listing contacts
- Cross-origin resource sharing (CORS) support
- Customizable photo directory and URL handling

## Technologies Used
- Spring Boot for backend development
- Spring Data JPA for data access
- Lombok for boilerplate code reduction
- CORS configuration for handling cross-origin requests
- Java for backend development

## Example Images
- **API Endpoints**:
    - Create, retrieve, update, and delete contact records.
    - Example of a contact record:
      ```json
      {
        "id": "uuid",
        "name": "John Doe",
        "email": "john.doe@example.com",
        "phone": "123-456-7890",
        "address": "123 Elm Street",
        "title": "Software Engineer",
        "status": "Active",
        "photoUrl": "http://localhost:8080/contacts/image/uuid.png"
      }
      ```

## Getting Started

### Prerequisites
- Java 17 or newer
- Maven (for building the project)
- An IDE or text editor of your choice

### Installation
1. Clone the repository:
    ```bash
    git clone <repository-url>
    cd contact-api
    ```

2. Build the project using Maven:
    ```bash
    mvn clean install
    ```

3. Run the application:
    ```bash
    mvn spring-boot:run
    ```

4. Open [http://localhost:8080](http://localhost:8080) with your browser to access the API.

### API Documentation
- **Create Contact**: POST `/contacts`
- **Get Contacts**: GET `/contacts`
- **Get Contact by ID**: GET `/contacts/{id}`
- **Update Contact**: PUT `/contacts`
- **Upload Photo**: PUT `/contacts/photo`
- **Get Photo**: GET `/contacts/image/{filename}`
- **Delete Contact**: DELETE `/contacts/{id}`


