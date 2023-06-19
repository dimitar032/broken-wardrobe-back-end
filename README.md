# Abstract
Backend implementation of the web platform for second hand clothing

# Roles:
## internal users (from the company)
- Admin
- Company sellers
## external users (outside from the company)
- Resellers (their product must be approve by our sellers)
- buyers (end users / normal users)

# Architecture
- Laravel 9 LTS (back) - PHP 8.1
- Angular 14 (front)
- SPA 

# Product Lifecycle
1. Product is received in the warehouse
2. Upload the product in the system (pictures/ buying price for our products/ price for reseller / brand / category of the product / selling price / when to be visible)
3. CRON - make the product available for reservation
4. first person that click is reserving the product
5. first person that have it reserver can purchase the product and the reservatioin is 15 minutes
6. the product is sold to the user
7. the user have 14 days to return the product (why)
8. product is reveiewed by the company resellers
9. product is available for reservation / or destroyed
