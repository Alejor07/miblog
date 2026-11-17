---
layout: post
title:  "Instalar Apache en Ubuntu Server"
date:   2026-10-01 10:00:00
categories: servidores
tags: [apache, ubuntu, http]
---
En esta práctica instalamos el servidor web Apache y comprobamos que respode en el puerto 80.

## Instalación 

```bash
sudo apt update
sudo apt install apache2
sudo systemctl enable --now apache2
```

## Comprobacion

```bash
systemctl status apache2
curl -I http://localhost
```

Si todo va bien, el navegador mostrara la pagina *It works!*
![Logo apache](/assets/images/posts/apache/apache-logo.png)