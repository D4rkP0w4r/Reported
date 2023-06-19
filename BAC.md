# Broken Access Control in FUEL-CMS-1.5.2

1.  Login to user have permission user(create, edit,... users)

![image](https://github.com/D4rkP0w4r/Reported/assets/79050415/4082aac3-3b43-4967-9970-7d87fc8fa3db)

2. Go to https://localhost/fuel/users/toggle_off/1/active

![image](https://github.com/D4rkP0w4r/Reported/assets/79050415/d813f79b-4970-4782-b0ee-0c1ce6cb34c7)

3. The admin account has been inactive
![image](https://github.com/D4rkP0w4r/Reported/assets/79050415/a16d3d9e-f4f3-4004-b1c5-8cf56cacdeb5)

### Impact 
* Attacker can active or inactive any accounts registerd in system
