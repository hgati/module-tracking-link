# Magento2 Tracking Link

[![Total Downloads](https://poser.pugx.org/hgati/module-tracking-link/downloads)](https://packagist.org/packages/hgati/module-tracking-link)
[![Latest Stable Version](https://poser.pugx.org/hgati/module-tracking-link/v/stable)](https://packagist.org/packages/hgati/module-tracking-link)

Extension add Tracking Url in Shipment Email.

Native shipment email doesn’t include a clickable tracking number link, just plain text one. The customer has to copy and then go to the courier site to get the tracking information. The extension make the tracking number a clickable link that will bring them to the carriers site and display the tracking information.
The extension supports all couriers which support shipping tracking.

## Install

#### Install via Composer (recommend)

    ```bash
    composer require hgati/module-tracking-link

    php bin/magento setup:upgrade
    php bin/magento setup:di:compile
    php bin/magento setup:static-content:deploy (optional)    
    ```
### Configuration

In the Magento Admin Panel go to *Stores > Configuration > Hgati > Tracking Settings > Tracking Service Url*.

<img alt="Magento2 Tracking Link" src="https://karliuka.github.io/m2/tracking-link/config.png" style="width:100%"/>

## Usage
#### Shipment Email
<img alt="Magento2 Tracking Link" src="https://karliuka.github.io/m2/tracking-link/email.png" style="width:100%"/>

#### Service Tracking Page
<img alt="Magento2 Tracking Link" src="https://karliuka.github.io/m2/tracking-link/ups.png" style="width:100%"/>

## Uninstall

#### Remove database data

```bash
php bin/magento module:uninstall -r Hgati_TrackingLink
```