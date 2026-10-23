Day 1 Notes
Application tested: [https://www.saucedemo.com/]
Date: 23 October 2026
Browser: Google Chrome 
SDLC vs STLC summary
1. SDLC is the process of building software: planning, requirement analysis, design, coding, testing, deployment, and maintenance.
2. STLC is the process of testing software: requirement analysis, test planning, test case design, test environment setup, test execution, test reporting, and test closure.
3. SDLC focuses on developing quality software, while STLC verifies and validates software quality.
4. STLC is part of the overall software development process and is closely connected to the testing phase of SDLC.
5. QA should start at the requirements stage, not after coding, because early defects are generally cheaper to fix.
Observations
#	Area	Steps	Expected	Actual	Result	Severity
1	Standards	Use the standard user account and test the application	Standards should work consistently	Sometimes working, sometimes not working	Bug	Major
2	Sorting	Sort A–Z, Z–A, price low–high, and price high–low	Items should reorder correctly	All four sorting options are working	Pass	—
3	Cart	Add and remove all products	Cart should update correctly	Add to Cart and Set Successfully are working; all products were tested, including removal	Pass	—
4	Checkout	Enter first name, last name, postal code, payment information, and shipping information	Checkout should complete and confirm the order	Checkout completes, displays “Thank you for ordering,” and PDF generation works	Pass	—
5	Menu	Open the menu	Menu should display all available options	Menu has 5 options	Observation	—
6	Dynamic Catalog	Open the Dynamic Catalog	Catalog should display all available options	Dynamic Catalog has 3 options	Observation	—
7	Lazy Load	Open Lazy Load and test sorting	Products should be sorted correctly	Sorting options are not working	Bug	Major
8	Lazy Load	Open the Lazy Load page	All available items should display	All items are showing	Pass	—
9	Lazy Load	Check product listings and sizes	Items should be unique and product information should be correct	Duplicate items are present, including two items in L size	Bug	Minor
10	Lazy Load	Open the Lazy Load page and inspect products	Relevant products should display correctly	Blue Light T-shirts and a Backpack are displayed	Observation	—
11	Spinner	Open the Spinner page	Products should display as expected	Shows the same items as Lazy Load, but in a smaller amount	Observation	—
12	Slider	Open the Slider page	Multiple items should display	Only one item is displayed, although multiple items are included	Bug	Major
13	Dynamic Catalog	Open all three Dynamic Catalog options	Add to Cart should be available if required	None of the three options has an Add to Cart option	Bug	Major
14	Menu	Open the menu and click About	About page should load successfully	Displays a 403 Forbidden error	Bug	Major
15	Menu	Click Reset App State	Application state should reset successfully	Reset App State is working	Pass	—
16	Menu	Click Log Out	User should log out successfully	Log Out is working	Pass	—
17	All Items	Open All Items and check T-shirt and Jacket sizes	Product sizes should display consistently where applicable	T-shirts and Jackets do not show sizes, whereas the Dynamic Catalog displays sizes	Bug	Minor

Note: Severity levels are preliminary estimates. Confirm them against the application's requirements and the impact on users.
Per-user results
The following table is prepared for recording the results of testing each user account. The observations provided so far do not establish which issues occurred under each specific account, so those details remain unfilled.
User	Steps	Expected	Actual	Result	Severity
standard_user	Log in with valid credentials and test the main features	Login and features should work correctly	Some standards were reported to work inconsistently; sorting, cart, and checkout worked	Partial pass	To confirm
locked_out_user	Attempt to log in with the locked-out account	Login should be denied with an appropriate message	Not yet confirmed	Pending	—
problem_user	Log in and test products, cart, sorting, and checkout	Features should behave correctly	Not yet confirmed separately	Pending	—
error_user	Log in and test application features	Features should behave correctly	Not yet confirmed separately	Pending	—
visual_user	Log in and inspect layout, images, and product display	Visual elements should display correctly	Not yet confirmed separately	Pending	—
