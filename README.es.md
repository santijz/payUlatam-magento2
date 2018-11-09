# Modulo de Pago PayuLatam para Magento 2

*Otros idiomas del Readme: [Español](README.es.md),[English](README.md)

Integración PayuLatam para Magento 2

## Características
- Webcheckout (Unica integración disponible por ahora)
- Soporte a multi-tienda,
- Integración Inicial con el flujo de pago de Magento 2 (transaccioness, reintentos, etc.),
- Registro de acciones, errores, etc
- Modo de Prueba (Recuerde configurar los parametros de: http://developers.payulatam.com/es/web_checkout/sandbox.html para pruebas sandbox)


## Configuración en el panel de PayuLatam

"URL de Respuesta" debe apuntar a "yourdomain/payulatam/payment/end"

"URL de confirmación" debe apuntar a "yourdomain/payulatam/payment/notify"

Reemplace "sudominio" con la direccion de su tienda. Ej. "tienda.com/payulatam/payment/end".


## Configuración en Panel de Magento 2

La configuración puede encontrarse en "Stores > Configuration > Sales > Payment Methods > Imagina PayuLatam."

## Como instalar
Desde la linea de comandos en la raiz de magento:
```ssh
composer require imagina/magento2-payulatam
php bin/magento setup:upgrade
php bin/magento setup:di:compile
```

Mas información:  https://www.imaginacolombia.com
