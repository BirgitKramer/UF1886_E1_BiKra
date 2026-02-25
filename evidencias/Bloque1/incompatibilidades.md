# Incompatibilidades

## Mostrar contenido de `__manifest__.py`
`sed -n '1,200p' addons/dev/custom_sale_codes/__manifest__.py`
`sed: can't read addons/dev/custom_sale_codes/__manifest__.py: No such file or directory`

### Carga de modulo en DEV
```
sed -n '1,200p' addons/dev/custom_sale_codes/__manifest__.py
{
"name":"Custom Sale Codes (Report)",
    "version": "1.0.0",
    "category": "Sales",
    "summary": "Anade referencia interno y codigo de barras al reporte de pedidos",
    "depends": ["sales"],
    "data": [
        "views/sale_report_xml"
    ],
    "installable": True,
    "application": False,
    "license": "LGP-3"
}
