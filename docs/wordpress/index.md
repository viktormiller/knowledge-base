# Wordpress

## WP-CLI

### Get option value

```bash
wp option get woocommerce_amazon_payments_advanced_settings --format=json
```

### Update option value

```bash
wp option update woocommerce_amazon_payments_advanced_settings '{"sandbox":"yes","merchant_id":"YOUR_MERCHANT_ID",...}' --format=json
```
