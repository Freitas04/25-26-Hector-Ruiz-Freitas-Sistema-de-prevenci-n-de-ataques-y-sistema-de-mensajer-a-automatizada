# 25-26-Hector-Ruiz-Freitas-Sistema-de-prevenci-n-de-ataques-y-sistema-de-mensajer-a-automatizada
Ficheros Configuración Servidor
/etc/netplan/00-wazuh-net.yaml:	configuración de red	Configuración manual con IP 192.168.10.10
/var/ossec/etc/ossec.conf:	principal del manager	Active Response, Integración Telegram, ajustes del ruleset
/var/ossec/integrations/telegram.py:	integración Python	Envío de alertas automáticas a Telegram
/var/ossec/etc/rules/local_rules.xml:
/var/ossec/etc/rules/:	reglas personalizadas	reglas añadidas
(   |   |   ├─ firewall-drop
│   │   │   ├─ disable-account
│   │   │   ├─ route-null
│   │   │   └─ restart-wazuh)
/etc/postfix/main.cf:	SMTP de Gmail	Configuración de correo

Ficheros Configuración Clientes
/var/ossec/etc/ossec.conf:	principal del manager	Active Response, Integración Telegram, ajustes del ruleset
/var/ossec/ruleset/sca/cis_ubuntu24-04.yml	archivo SCA	si lo copias a los clientes
