PHP Drupal 9 API assessment

Expose a JSON API endpoint that consumes a custom Content Type.  The custom content type could be a Product List (sku, name, description, price)

## Steps to Use Lando with Drupal 9 application

1. You need to clone this Drupal 9 project repository.

```
git clone https://github.com/reggiestain/lando--drupal9-api-assessment.git
```

2. Change the directory to the cloned repository.

```
cd lando--drupal9-api-assessment
```
3. Download and install project dependencies by running the below from the project directory.

```
composer install
```

3. Start your app using the lando start command. Before you begin, you can change some parameters in .lando.yml as per the need of your application.

```
lando start
```

After running the above command information about the application is displayed. Example APPSERVER URLS below


```
 APPSERVER URLS  https://localhost:53360
                 http://localhost:53361
                 http://drupal9-api-assessment.lndo.site/
                 https://drupal9-api-assessment.lndo.site/
```
Go to Postman, select GET method, enter your request URL
http://lando-drupal9-api-assessment.lndo.site/api/json/node/product_list and click the Send button.

![alt text](https://github.com/reggiestain/lando--drupal9-api-assessment/blob/master/postman-screenshot.PNG?raw=true)
