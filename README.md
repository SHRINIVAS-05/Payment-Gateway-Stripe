
# Stripe Payment Integration  

This repository demonstrates the integration of Stripe Payment Gateway into a web application. The implementation allows seamless payment processing, providing users with a secure and reliable transaction experience.  

## Features  
1. **Product-Based Payments**:  
   - Each transaction requires the following details:  
     - Product Name  
     - Quantity  
     - Currency (e.g., USD, EUR, etc.)  
     - Amount in smallest currency unit (e.g., cents for USD, paisa for INR).  

   - Example: For a $100 transaction, the amount should be provided as `100 * 100 = 10,000` cents.  

2. **Stripe-Provided Data**:  
   - Session URL for redirecting the user to Stripe Checkout.  
   - Session ID for transaction identification.  
   - Status and Message about the payment.  

3. **Test Card**:  
   - Stripe provides a test card for development purposes.  
   - Example test card details:  
     - Card Number: `4242 4242 4242 4242`  
     - Expiry Date: `Any future date`  
     - CVC: `Any 3-digit number`  

4. **Secure API Integration**:  
   - Requires a **private key** provided by Stripe.  
   - Ensure that the key is securely stored and not exposed in the repository or client-side code.  

## How It Works  
1. Provide product details and transaction details (name, quantity, currency, amount).  
2. Use Stripe's API to create a session.  
3. Retrieve the session details (URL, session ID, status, etc.).  
4. Redirect the user to the Stripe Checkout page using the session URL.  
5. Use the Stripe dashboard or webhook integration to track payment status and events.  

## Installation and Setup  

### Prerequisites  
- **Java Version**: JDK 17 or higher  
- **Dependencies**:  
  - Lombok  
  - Stripe  
  - Thymeleaf  

- **Development Environment**:  
  - Any IDE like Eclipse, IntelliJ IDEA, or Spring Tool Suite (STS).  

- **Testing Tool**:  
  - Postman for API testing and validation. 
