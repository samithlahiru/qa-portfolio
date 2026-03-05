# User Stories – Authentication (Sign-Up & Sign-In)

## 1. Access the Sign-Up Page
**ID:** 1.1  
**As a** new or returning user  
**I want** to access the Sign-Up page from the homepage or redirect after session timeout  
**So that** I can create a new account or log in  

**Acceptance Criteria:**  
1. **Navigation from homepage:**  
   - Given I am on the homepage  
   - When I click the **Sign-Up** button  
   - Then I should be redirected to the Sign-Up form page  

2. **Already logged-in user:**  
   - Given I already have an active session  
   - When I try to visit the Sign-Up page  
   - Then I should be redirected to the homepage  

3. **Session expired:**  
   - Given my session expired due to inactivity  
   - When I click any button  
   - Then I should be prompted to log in before accessing Sign-Up  

---

## 2. Access the Sign-In Page
**ID:** 1.2  
**As a** returning user  
**I want** to access the Sign-In page from the homepage or after session timeout  
**So that** I can log in to my account  

**Acceptance Criteria:**  
1. **Navigation from homepage:**  
   - Given I am on the homepage  
   - When I click the **Sign-In** button  
   - Then I should be redirected to the Sign-In form page  

2. **Already logged-in user:**  
   - Given I already have an active session  
   - When I try to visit the Sign-In page  
   - Then I should be redirected to the homepage  

3. **Session expired:**  
   - Given my session expired due to inactivity  
   - When I try to perform any action  
   - Then I should be prompted to log in before proceeding  
