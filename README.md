# Magento 2 - Simple Stack


| Stack | Version |
|--|--|
| Apache | 2.4.25 |
|PHP|7.1.25|
| Redis | 4.0.11 |
| MariaDB | 15.1 Distrib 10.3.11-MariaDB |

## How to connect to Apache2/PHP container?
    docker exec -it "apache-container-name" bash

## How to connect to Mariadb?

    docker exec -it "mariadb-container-name" mysql -umagento -pmagento

## How to download Magento 2?

 - Inside ***src*** folder, download from official repository via composer or zip file in: https://magento.com/tech-resources/download
 - Install Magento using this simple command:

     bin/magento setup:install --base-url=http://localhost/ \
		        --db-host=db \
		        --db-name=magento \
		        --db-user=magento \
		        --db-password=magento \
		        --admin-firstname=Developer \
		        --admin-lastname=Magento2 \
		        --admin-email=admin@example.com \
		        --admin-user=admin \
		        --admin-password=admin123 \
		        --language=en_US \
		        --currency=USD \
		        --timezone=America/Chicago \
		        --use-rewrites=1 \
		        --backend-frontname=admin \
		        --use-sample-data


