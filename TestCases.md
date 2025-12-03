# Test Cases — Saucedemo Web App

---

## 🟢 LOGIN MODULE (8 Test Cases)

### TC01 — Successful Login
**Steps:**  
1. Navigate to login page  
2. Enter valid username/password  
3. Click Login  
**Expected:** User lands on inventory page

### TC02 — Login with invalid password
Expected: Error message displayed

### TC03 — Login with blank username
Expected: “Username is required”

### TC04 — Login with blank password
Expected: “Password is required”

### TC05 — Login with locked user
Expected: "User is locked out"

### TC06 — Case sensitivity test
Expected: Should NOT log in

### TC07 — Login button without inputs
Expected: Validation error

### TC08 — Slow network login
Expected: Loader shown, user logs in successfully

---

## 🟢 PRODUCT PAGE (8 Test Cases)

### TC09 — Verify product list loads
Expected: 6 items displayed

### TC10 — Sort A–Z
Expected: Items alphabetically sorted

### TC11 — Sort Z–A
Expected: Reverse sort

### TC12 — Sort Price Low → High
Expected: Correct order

### TC13 — Open product detail
Expected: Product info loads

### TC14 — Back button returns to inventory
Expected: Inventory restores correctly

### TC15 — Add product to cart from list
Expected: Button changes to “Remove”

### TC16 — Add product to cart from details page
Expected: Cart count = 1

---

## 🟢 CART MODULE (7 Test Cases)

### TC17 — Add multiple products
Expected: Cart count increases correctly

### TC18 — Remove product from cart
Expected: Item removed

### TC19 — Verify cart total is correct
Expected: Sum matches product prices

### TC20 — Continue shopping
Expected: Returns to inventory page

### TC21 — Cart persists after page refresh
Expected: Items remain

### TC22 — Cart empty state
Expected: “Your cart is empty”

---

## 🟢 CHECKOUT MODULE (7 Test Cases)

### TC23 — Checkout step 1 loads
### TC24 — Missing first name
Expected: Validation error

### TC25 — Missing postal code
Expected: Validation error

### TC26 — Valid checkout information
Expected: User moves to step 2

### TC27 — Validate item summary
Expected: Items & prices correct

### TC28 — Finish checkout
Expected: “Order Completed” page

### TC29 — Back button during checkout
Expected: Should not break workflow

---

## 🟢 LOGOUT (1 Test Case)

### TC30 — Successful Logout
Expected: Redirected to login page
