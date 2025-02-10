# Test Task, Mariia Namynanik

Test cases for endpoint {{host}/pet/deletePet}  
https://petstore.swagger.io/#/pet/deletePet

Some test cases include assumptions or comments due to missing requirements in the provided documentation!!!

---

### Test Case № 1:
**Title:** Successful Delete a pet with valid ID

**Preconditions:**  
1) The link https://petstore.swagger.io/#/pet/deletePet is open in the browser
2) Created animal
3) Api key - "special-key"

**Steps:**  
1) Send a POST request with parameters:  
  Api key with Preconditions  
  PetId created animal


**Expected Result:**  
1) Status code of the response: 200 OK.  
2) The pet successful Delete.  
 

---

### Test Case № 2:
**Title:** Delete a pet with invalid ID  

**Preconditions:**  
1) The link https://petstore.swagger.io/#/pet/deletePet is open in the browser
2) Api key - "special-key"

**Steps:**  
1) Send a POST request with parameters:  
  Api key with Preconditions  
  PetId invalid ID

**Expected Result:**  
1) Status code of the response: 404.  
2) The response body contains information about the error, such as:  
   `"Requested resource could not be found. "` 