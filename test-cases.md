# Test Cases: Swag Labs (saucedemo.com)

Fill in **Actual result** and **Status** (Pass / Fail) as you run each test. Screenshot any failure and report it in `bug-reports.md`.

|ID|Module|Title|Steps|Expected result|Actual result|Status|
|-|-|-|-|-|-|-|
|TC-01|Login|Login with valid user|Enter standard\_user / secret\_sauce, click Login|Products page opens|page opens sucessfully|pass|
|TC-02|Login|Wrong password|Enter standard\_user / wrong, click Login|Error: username and password do not match|Epic sadface: Username and password do not match any user in this service|pass|
|TC-03|Login|Locked out user|Login as locked\_out\_user|Error: user has been locked out|not tested|pending|
|TC-04|Login|Empty username|Leave username empty, enter password, Login|Error: Username is required|Epic sadface: Username is required|pass|
|TC-05|Login|Empty password|Enter username, leave password empty, Login|Error: Password is required|Epic sadface: Password is required|pass|
|TC-06|Login|Both fields empty|Click Login with empty fields|Error: Username is required|Epic sadface: Username is required|pass|
|TC-07|Login|Username case sensitivity|Enter STANDARD\_USER / secret\_sauce|Login rejected|login sucessfully|pass|
|TC-08|Login|Open inventory without login|Open /inventory.html directly when logged out|Error: you can only access it when logged in|make login first|pass|
|TC-09|Login|Logout|Login, open menu, click Logout|Login page shown|login page shown|pass|
|TC-10|Inventory|Product list|Login and view products|6 products shown with image, name, price, button|Products page opened with 6 products|pass|
|TC-11|Inventory|Sort name A to Z|Choose Name (A to Z)|Products in ascending name order|sorts product as intended|pass|
|TC-12|Inventory|Sort name Z to A|Choose Name (Z to A)|Products in descending name order|sorts in descending order|pass|
|TC-13|Inventory|Sort price low to high|Choose Price (low to high)|Prices in ascending order|prices sorted(ascending order) sucessfully|pass|
|TC-14|Inventory|Sort price high to low|Choose Price (high to low)|Prices in descending order|price sorted successfully in descending order|pass|
|TC-15|Inventory|Open product details|Click a product name|Details page shows correct name, price, description|displayed correct details|pass|
|TC-16|Inventory|Back to products|On details page click Back to products|Products page shown|product page shown sucessfully|pass|
|TC-17|Cart|Add one item|Click Add to cart on one product|Button becomes Remove, cart badge shows 1|||
|TC-18|Cart|Add multiple items|Add 3 products|Badge shows 3|||
|TC-19|Cart|Remove from products page|Add item, click Remove|Badge disappears, button back to Add to cart|||
|TC-20|Cart|Remove from cart page|Add item, open cart, click Remove|Item removed from cart|||
|TC-21|Cart|Cart keeps items|Add item, go to another page, open cart|Item still in cart|||
|TC-22|Cart|Continue shopping|In cart, click Continue Shopping|Products page shown|||
|TC-23|Checkout|Valid checkout details|Cart, Checkout, enter name and postal code, Continue|Overview page opens|||
|TC-24|Checkout|First name missing|Leave first name empty, Continue|Error: First Name is required|Error: First Name is required|pass|
|TC-25|Checkout|Last name missing|Leave last name empty, Continue|Error: Last Name is required|Error: Last Name is required|pass|
|TC-26|Checkout|Postal code missing|Leave postal code empty, Continue|Error: Postal Code is required|Error: Postal Code is required|pass|
|TC-27|Checkout|Cancel at step one|Click Cancel on checkout info page|Returns to cart|Returns to cart|pass|
|TC-28|Checkout|Price calculation|On overview, add item prices, compare to Item total and Total|Item total correct, tax and total correct|Item total correct, tax and total correct|pass|
|TC-29|Checkout|Complete order|Click Finish on overview|Order complete message shown||pass|
|TC-30|Checkout|Cart empty after order|Complete order, check cart badge|Cart is empty||pass|
|TC-31|Checkout|Checkout with empty cart|Open cart with no items, click Checkout|Record the behaviour; expected: blocked or warned||pass|
|TC-32|Menu|Reset App State|Add items, menu, Reset App State|Cart emptied||pass|
|TC-33|Special user|problem\_user product images|Login as problem\_user, view products|Each product shows its own image||pass|
|TC-34|Special user|performance\_glitch\_user login|Login as performance\_glitch\_user|Login completes; note time taken||pass|



