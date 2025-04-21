# Conectando tu WordPress a un CRM

Tu WordPress puede ser un gran aliado de tu CRM, surtiéndole de mucha información, como nuevos contactos y leadscorings. Y esto también funciona al revés, proveyendo a tu WordPress con información sobre el contacto que le ayude a vender.

Pero primero debes **aprender a conectarlos**.

LOGO DE CREADO SIN IA

LOGO FEMENINO genérico.
---

En esta ponencia veremos las diferentes formas que permiten que se comuniquen entre sí estos dos elementos fundamentales de tu estrategia de marketing con ejemplos sencillos de algunos de los CRM más populares, como:

* ActiveCampaign
* HubSpot
* ZohoCRM
* Clientify
* Mautic
* Salesforce

Trataremos de ver formas de conexión que impliquen programación y ejemplos que no, para ver todas las posibilidades. 

---

# Reglas fundamentales

* Tu CRM debe tener una API y cuanto más completa mejor. Con buena documentación y a poder ser con alguna librería ya desarrollada en el lenguaje que vayas a usar.
* Sabed si vuestro hosting puede conectarse a otros servidores. No es muy normal, pero a veces están capados, si te todo con instituciones y grandes empresas preocupadas con la ciberseguridad. Hablad con el hosting para que meta la IP del CRM en algún tipo de lista blanca.
* Tratad de saber si tienen servidores europeos. Como están las cosas puede ahorraros muchos problemas si en el futuro hay que migrar todo a sistemas en Europa. 
* XXX

Muchos CRM dan periodos de prueba gratuitos de 15 días o similar. No es una perdida de tiempo pedir esas pruebas y hacer algunos tests básicos.

Migrar el día de mañana de un CRM a otro porque no cumple todas nuestras expectativas va a llevarte más tiempo que hacer unas pruebas básicas con el periodo de prueba.

---

# El código de tracking

La forma principal de conectar tu WordPress y tu CRM es un código de tracking.

Suele ser meter un código paracido a Analytics en todas las páginas de la web. Hay muchas formas para meter estos códigos.

* Directa en header.php del tema.
* Con el hook wp_header en el functions.php.
* Hay temas que te permiten meter código JavaScript en las cabeceras web.
* Muchos CRM tienen plugins con integraciones básicas del código de trackeo.
* Si ya tenéis TagManager podéis configurarlo como una etiqueta más.

## Obligaciones legales

Muchos de estos códigos de tracking dejan cookies, así que tendrás que montarlo dentro de su sistema de gestión de cookies y dar información en el aviso de cookies.

## ¿Cómo trabajan estos códigos?

Estos códigos detectan e identifican a los usuarios a partir de los clicks en emails que hayan sido enviados desde el CRM.

Una vez clican y sin identificados dejan una cookie que nos permite rastrearlo por la web.

Sin ese primer click en una newsleter no hay identificación y no se rocege información. Un usuario en nuestro CRM si entra directamente en nuestra desde un ordenador sin la cookie no será detectado.

## ¿Qué permiten estos códigos solo con meterlos?

Este simple código os da ya mucho potencial entre muchas de las opciones podemos:

* Saber las paginas que visita.
* XXX

---

# URL de tracking de clics

XXX

Mirar cansadito en el Gmail.

---

# Conexión directa a la API o crear un middleware

XXX

---

# Formularios

La forma mas común de conexión entre WordPress y Un CRM es mediante formularios. Está conexión se puede hacer mediante diferentes formas.

## Incrustados

La mayoría de CRM dan códigos para incrustar formularios en tu web. Son códigos muy sencillos de usar, creas el formulario y cortas y pegas el código que te dan en tu web, en páginas, widgets, ...

**Ventajas:**

* Muy fácil de crear e integrar.
* La conexión es directa.
* Ellos se encargan de meter la cookie de rastreoo similares para poder seguir al usuario.

**Desventajas:**

* Cuando quieres meter campos especiales que no están en el CRM, te obliga a crear campus personalizados en el CRM para guardar esa información. A la larga creas montones de campos que casi mi se usan.
* No tienen buena integración en el diseño de tu WordPress Y suelen quedar un poco pegote.
* No permiten conectar a terceros. Los formularios incustrados se conectan difícilmente con elementos de terceros. Tengo una fundación de una empresa grande que todos los contactos recogidos con los formularios deben registrarse en el CRM que usan ellos (Clientify) y con el de la empresa matriz (Salesforce). Los formularios incrustados de Clientify no permiten hacer una conexión también a Salesforce cumpliendo los requerimientos que Salesforce exige.

## Conectados con un plugin

XXX

**Ventajas:**

* XXX

**Desventajas:**

* XXX

## Conectados con un desarrollo propio

XXX

**Ventajas:**

* XXX

**Desventajas:**

* XXX

## Mixto

XXX

**Ventajas:**

* XXX

**Desventajas:**

* XXX

---

# Consejos

* **Cread un campo de fecha de última modificación.** Los CRM suelen guardar está información, pero no discriminan entre conexiones por API y directamente por web. Con este campo personalizado tendréis control de qué contactos habéis tocado desde WordPress y cuáles han sido tocados de otras formas.
* **Usad las notas.** Muchos CRM te permiten crear notas de cada contacto, usad esas notas para guardar información variada, por ejemplo, el contenido de las áreas de texto de un formulario. Ponéis un título explicativo y luego el texto que escribió la persona que relleno el formulario. Siempre que se pueda, **no creéis campos específicos para ese tipo de cosas**.
* **Si puedes hacerse con una automatización del CRM, mejor que programándolo:** al conectar se puede hacer que el script que desarrolléis haga todas las tareas, como meter etiquetas, apuntar a listas, meter puntos en un LeadScoring, etc. O simplemente que lance un disparador de una automatización y esta ejecute todo lo anterior. Piensa que cambiar la programación solo podrá hacerlo una desarrolladora y cambiar una automatización con un interfaz gráfico, puede hacerlo cualquier persona de marketing con unos conocimientos básicos.

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