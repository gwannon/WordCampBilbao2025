# Conectando tu WordPress a un CRM

Tu WordPress puede ser un gran aliado de tu CRM, surtiéndole de mucha información, como nuevos contactos y leadscorings. Y esto también funciona al revés, proveyendo a tu WordPress con información sobre el contacto que le ayude a vender.

Pero primero debes **aprender a conectarlos**.

---

En esta ponencia veremos las diferentes formas que permiten que se comuniquen entre sí estos dos elementos fundamentales de tu estrategia de marketing con ejemplos sencillos de algunos de los CRM más populares, como:

* ActiveCampaign
* HubSpot
* ZohoCRM
* Clientify
* Mautic
* Salesforce

Trataremos de ver formas de conexión que impliquen programación y ejemplos que no para ver todas las posibilidades. 

---

# Reglas fundamentales

* Tu CRM debe tener una API y cuanto más completa mejor. Con buena documentación y a poder ser con alguna librería ya desarrollada en el lenguaje que vayas a usar.
* Sabed si vuestro hosting puede conectarse a otros servidores. No es muy normal, pero a veces falla. Hablad con el hosting para que meta la IP del CRM en algún tipo de lista blanca.
* Tratad de saber si tienen servidores europeos. Como están las cosas puede ahorraros muchos problemas si en el futuro hay que migrar todo a sistemas en Europa. 
* XXX

Muchos CRM dan pruebas gratuitas de 15 días o similar. No es una perdida de tiempo pedir esas pruebas Migrar el día de mañana de un CRM a otro porque no cumple todas nuestras expectativas va a llevarte más tiempo que hacer unas pruebas básicas con el periodo de prueba.

---

# El código de tracking

XXX

## Obligaciones legales

Muchos de estos códigos de tracking dejan cookies, así que tendrás que montarlo dentro de su sistema de gestión de cookies y dar información en el aviso de cookies.

---

# URL de tracking de clics

XXX

---

# Conexión directa a la API o crear un middleware

XXX

---

# Formularios

## Incrustados

XXX

## Conectados con un plugin

XXX

## Conectados con un desarrollo propio

XXX

## Mixto

XXX

---

# Consejos

* **Cread un campo de fecha de última modificación.** Los CRM suelen guardar está información, pero no discriminan entre conexiones por API y directamente por web. Con este campo personalizado tendréis control de qué contactos habéis tocado desde WordPress y cuáles han sido tocados de otras formas.
* **Usad las notas.** Muchos CRM te permiten crear notas de cada contacto, usad esas notas para guardar información variada, por ejemplo, el contenido de las áreas de texto de un formulario. Ponéis un título explicativo y luego el texto que escribió la persona que relleno el formulario. **No creéis campos específicos para ese tipo de cosas**.
* **Si puedes hacerse con una automatización del CRM, mejor que programándolo:** XXX

---

# Jorge Monclús 

XXX

---

# Enlaces

* [Ponencia](https://github.com/gwannon/WordCampBilbao2025) XXX

## Plugins

* [FormsCRM](https://es.wordpress.org/plugins/formscrm/) XXX

## Librerías

* [PHPClientifyAPI](https://github.com/gwannon/PHPClientifyAPI) XXX
* [HPActiveCampaignAPI](https://github.com/gwannon/PHPActiveCampaignAPI) XXX