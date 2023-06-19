# Broken Access Control in FUEL-CMS-1.5.2
1. login to user

![image](https://github.com/D4rkP0w4r/Reported/assets/79050415/2b83915f-2574-4e6b-9207-242d1e129985)

2. Get the user id of that page (page_id can guess just 1,2,3,...)

![image](https://github.com/D4rkP0w4r/Reported/assets/79050415/caa28e08-fcb6-4d05-b170-7d16d111ba57)

3. Attacker can active and inactive any users
* https://localhost/fuel/users/toggle_on/<user_id>/active (on is active)
* https://localhost/fuel/users/toggle_off/<user_id>/active (off is inactive)

![image](https://github.com/D4rkP0w4r/Reported/assets/79050415/c02b628d-8cbb-4b4e-a52d-6b9103e71f57)

4. User has been inactive

![image](https://github.com/D4rkP0w4r/Reported/assets/79050415/903f0efd-ccb2-46d7-99be-0e19b618a1ee)

* Attacker can inactive superadmin account 
