# CSRF in FUEL-CMS-1.5.2
1. login to admin create new page

![image](https://github.com/D4rkP0w4r/CVEs/assets/79050415/707e9c7f-cae9-47b8-924e-826b311ac08a)

2. Get the page_id of that page (page_id can guess just 1,2,3,...)

![image](https://github.com/D4rkP0w4r/CVEs/assets/79050415/42591260-9bc2-433e-9ae1-4967cebe9872)

4. Login to user

![image](https://github.com/D4rkP0w4r/CVEs/assets/79050415/349a4895-6e91-4cfc-9fa8-0184b5915330)

5. Trick victims go to this malicious link
* (become private page) https://localhost/fuel/pages/toggle_off/<page_id>/published
* (become public page) https://localhost/fuel/pages/toggle_on/<page_id>/published

![image](https://github.com/D4rkP0w4r/CVEs/assets/79050415/e002d1f4-c36d-4489-be3f-6738f2bcf190)
![image](https://github.com/D4rkP0w4r/CVEs/assets/79050415/4166cc91-1968-4dda-81e4-c4041ca83b63)

--> Block, navigation, sitevariables have the same vulnerability.
