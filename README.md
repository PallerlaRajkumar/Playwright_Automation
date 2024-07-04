# Playwright_Automation
TASK:
Please use Playwright w/Typescript and make tests run parallelly.
So, we have left the cases open-ended for you.
1. Login: Visit amazon.in and login into site. Run login as first test and only once, if it fails rest
of the tests should not even start.
2. Search: search for the term “shoes”, you would need to verify that the values on the search
page are actually searched for shoes.
3. Applying Filters: You need to apply at least two filters and make sure that these filters are
applied and the results are being filtered logically.
4. Product Details page: Once you have identified the above two workflows, make sure to
validate the details of a particular product and then add it to the cart.



Run the tests using the commands on **individual test** scripts:

**npx playwright test ./tests/search.test.ts** 

**npx playwright test ./tests/filters.test.ts** 

**npx playwright test ./tests/product-details.test.ts** 

To Run All Tests in a **Single GO:**

**npx playwright test**

### 1. filters.test.ts 

**Purpose:**

 The script tests the functionality of applying brand filters on Amazon's search results page. 
 
 **Key Actions:** 
 
- Navigates to Amazon's homepage. 
- Searches for the term "shoes".
 - Waits for the search results to load.
 - Applies the "Puma" and "Adidas" brand filters. 
- Verifies that the filters are applied correctly. 

**Details:**

 - Uses Playwright for browser automation.
 - Logs HTML of the sidebar for debugging.
 - Increases timeouts to handle network delays. 
- Verifies the application of filters by checking the page elements


### 2. product-details.test.ts
 **Purpose:** 
The script tests the functionality of viewing product details and adding a product to the cart on Amazon.

 **Key Actions:**
 
 - Navigates to Amazon's homepage. 
- Searches for the term "laptop". 
- Clicks on the first product in the search results.
 - Verifies the product details page is loaded. 
- Adds the product to the cart. 
- Verifies the product is added to the cart. 

**Details:** 

- Uses Playwright for browser automation
. - Handles various page elements and actions. 
- Increases timeouts to ensure actions are completed successfully.



### 3. search.test.ts 

**Purpose:** 

The script tests the search functionality on Amazon's homepage. 

**Key Actions:**

 - Navigates to Amazon's homepage. - Searches for the term "shoes". 
- Verifies the page title contains "Amazon". 
- Waits for search results to load. 
- Verifies that search results contain the keyword "shoe".

  
**Details:**

  
 - Uses Playwright for browser automation. 
- Checks visibility and content of search results. 
- Logs the number of search results and their titles.
