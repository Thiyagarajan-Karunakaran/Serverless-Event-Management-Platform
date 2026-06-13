# Serverless-Event-Management-Platform

## 📖 Introduction
A serverless full-stack Event RSVP Management System built on AWS that allows users to browse events, view event details, and submit RSVP responses. The application leverages scalable AWS services to provide robust backend APIs, relational and NoSQL databases, static website hosting, and fast content delivery through a CDN.

## 🛠️ Technologies Used
*   **Cloud & Infrastructure:** AWS Lambda, Amazon API Gateway, Amazon S3, Amazon CloudFront, Amazon VPC, Security Groups
*   **Databases:** Amazon RDS (MySQL), Amazon DynamoDB
*   **Frontend:** HTML5, CSS3, JavaScript
*   **Backend:** Node.js, MySQL2, AWS SDK v3
*   **Tools:** Postman

## ⚙️ How It Works

<img width="1423" height="663" alt="Screenshot 2026-06-13 at 2 01 03 PM" src="https://github.com/user-attachments/assets/85ef9591-d8e7-4dd5-9f68-eb1e636d481d" />

1.  **Frontend Delivery:** The user interface is built using HTML, CSS, and JavaScript, hosted on Amazon S3, and delivered quickly via Amazon CloudFront (CDN).
2.  **API Routing:** User requests are routed through Amazon API Gateway, which exposes secure REST API endpoints.
3.  **Backend Processing:** The API Gateway invokes an AWS Lambda function that acts as the core backend service.
4.  **Data Management:** 
    *   Event information (title, venue, date, description) is fetched from Amazon RDS (MySQL).
    *   RSVP responses and attendance statistics are processed and stored in Amazon DynamoDB for efficient retrieval.
5.  **Dynamic Rendering:** The Lambda function returns JSON responses to the client. JavaScript dynamically renders event cards, populates modals, updates live statistics, and submits RSVPs without page reloads.

## ✨ Features
*   **Event Browsing:** View all available events and retrieve detailed information for individual events via interactive modals.
*   **RSVP System:** Submit Yes/No responses with email validation to prevent duplicate entries.
*   **Live Statistics:** Display real-time RSVP statistics and view attendees grouped by response type.
*   **Dynamic UI:** Engaging event cards with banner images.
*   **Serverless Architecture:** Highly scalable and cost-efficient backend using AWS Lambda and API Gateway.
*   **Hybrid Database Model:** Seamless integration of both SQL (RDS) and NoSQL (DynamoDB) databases.
*   **Optimized Delivery:** Static website hosting with S3 and global content delivery via CloudFront with Cross-Origin Resource Sharing (CORS) support.

## Video

https://github.com/user-attachments/assets/57ed8310-7867-4988-b409-125b2a819e05

