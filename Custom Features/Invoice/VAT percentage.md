> ### Step 1: Modify the Invoice Template:
#### Navigate to the invoice template file in your OpenCart theme directory. Typically, this file is located at:

```
catalog/view/theme/your_theme/template/invoice/invoice.twig
```

> ### Step 2: Add Code to Display VAT Percentage:
#### Find the section in the invoice template where you want to display the VAT percentage. It's usually near the subtotal or total section. Then, add the following code snippet to retrieve and display the VAT percentage:

```
{% for product in products %}
{{ product.tax }}%
{% endfor %}
```
