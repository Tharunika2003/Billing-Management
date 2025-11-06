Tech Stack :
____________

Backend (Spring Boot)
- Java 17
- Spring Boot
- Spring Security + JWT Authentication
- Spring Data JPA + Hibernate
- MySQL Database
- Lombok
- Spring Mail (SMTP - Gmail)
- Razorpay Java SDK
  
Frontend (React.js)
- React 18
- React Router
- Axios (API calls)

Project Structure :
___________________

Backend -
BackendChillBilling/
 ├── src/main/java/com/chillbilling
 │   ├── controller      # Controllers
 │   ├── service         # Business logic
 │   ├── repository      # Database access
 │   ├── entity          # Entity classes
 │   ├── dto             # Data Transfer Objects
 │   └── validation      # Custom validations
 ├── src/main/resources
 │   └── application.properties
 └── pom.xml
 
Frontend -
FrontendChillBilling/
 ├── public/
 ├── src/
 │   ├── api/            # API integration
 │   ├── assets/         # Static files
 │   ├── components/     # Reusable components
 │   ├── context/        # Context API
 │   ├── routes/         # Page routes
 │   ├── App.jsx
 │   └── index.js
 └── package.json

Setup Instructions :
____________________

1. Clone the Repository - 
    git clone https://github.com/prabhas1401/Chill-Billing.git
    cd chill-billing
   
2. Backend Setup (Spring Boot) -
     Prerequisites:
      - Install Java 17
      - Install Maven
      - Install and run MySQL
        
    Configure Database
      spring.datasource.url=jdbc:mysql://localhost:3306/chill_billing
      spring.datasource.username=root
      spring.datasource.password=YOUR_PASSWORD
    Configure Mail (SMTP)
      spring.mail.username=your-email@gmail.com
      spring.mail.password=your-app-password
    Configure Razorpay
      razorpay.keyId=your-key-id
      razorpay.keySecret=your-secret-key
      razorpay.webhookSecret=your-webhook-secret

    Run Backend -
      cd BackendChillBilling
      mvn spring-boot:run
   
3. Frontend Setup (React.js)
    Prerequisites:
      - Install Node.js
      - Install npm
        
    Install Dependencies
      cd FrontendChillBilling
      npm install
   
   Run React App
      npm run dev


