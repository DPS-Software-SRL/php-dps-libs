# php-dps-libs
Librerías comunes a sistemas DPS
-

* guzzlehttp/guzzle
* vlucas/phpdotenv
* cekurte/environment
* lcobucci/jwt
* kint-php/kint
* smarty/smarty
*
* dps-software-srl/php-mysql-lib
* dps-software-srl/php-mailjet-lib
* dps-software-srl/php-csrf-lib
* dps-software-srl/php-smarty-lib


# Archivo .env ideal para utilizar con estas librerias    
---
```
ENVIRONMENT   = "DEV" # DEV | TEST | PROD
HOST          = "localhost"
PATH_ROOT     = "/var/www/html" 
PATH_NOPUBLIC = "/var/www/nopublic"
PATH_LOG      = ${PATH_NOPUBLIC}/logs

ERROR_LOG_ENABLED   = true
ERROR_LOG_TO_SCREEN = false
ERROR_END_SCRIPT    = false

LOCALE_TIME    = "es"
LOCALE_NUMERIC = "en"
TIMEZONE       = "Etc/GMT+3"

IP_HABILITADAS = "" 

MYSQL_SERVER  = "mysql"
MYSQL_USER    = "root"
MYSQL_PASS    = "root"
MYSQL_BASE    = "db_pumaturnado"
MYSQL_PORT    = "3306"
MYSQL_TZ      = "-3:00"
MYSQL_LC_MS   = "es_AR"
MYSQL_LC_TN   = "es_AR"
MYSQL_LOG_SQL = false

# auth
AS_CALLBACK_URI        = "https://localhost"
AS_SHARED_JWT_SECRET   = "!VeKcA2teF^diZ3WqJ53wrieX9KF8mCSHHyCmm2h"
AS_BASE_URI            = "http://localhost:3000/auth/"
AS_API_INTERNAL_SECRET = "aaa"
AS_API_INTERNAL_URI    = "http://auth:3000/auth/"

SECRET_ANTI_CSRF = '7ggumCXCEHB$EgDv!pP'

KINT_ENABLED               = true
KINT_FIXED                 = true
KINT_SHOW_DEBUGINFO_AL_PIE = false

SEND_EMAILS       = true
# SEND_EMAILS_TO    = 'yo@softwaredps.com.ar'
SEND_EMAILS_TO_ONLY_FOR_DEBUG = "alguien@gmail.com"
MJ_FROM_NAME      = "PumaDigital"
MJ_FROM_EMAIL     = "noresponder.turnado@pumadigital.com.ar"
MJ_APIKEY_PUBLIC  = "35dbc2"  # TOKENS DE MAILJET
MJ_APIKEY_PRIVATE = "0c956"  # TOKENS DE MAILJET

SHOW_GIT_BRANCH  = true
```
