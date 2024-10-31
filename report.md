# Capitulo IV: Product Design

## 4.1. Style Guidelines


### 4.1.1. General Style Guidelines
**Branding:**

En la creación del logotipo, se emplearon los colores de la paleta principal, junto con la imagen de una olla que evoca la comida casera. Además, se seleccionó una tipografía que complementa perfectamente la temática.
<img src="/assets/LogoSC.png" width="300"/>
**Colors:**

Dado que el proyecto está enfocado en la preparación de comidas, realizamos la elección de una paleta de colores acorde al contexto. Así, pudimos escoger aquellos colores que creemos conveniente para la plataforma web:
<img src="/assets/brandcolor.png" width="300"/>
Nuestra paleta de colores principal está compuesta por un color dominante o primario (#E06B43) que es el más resaltante. Se utilizará para hacer énfasis en los textos, botones y en las páginas que contienen información relevante para el usuario. Este tono de naranja se asocia a la vitalidad, creatividad y sociabilidad, las cuales son características del público al que está dirigido la aplicación.

Dentro de los colores secundarios tenemos un tono naranja-amarillo brillante (#FFAC4A), que se utilizará para dar contraste, y el color crema (#FFE9C9) que es más suave y neutro, por lo que se usará para dar una sensación de simplicidad.
<img src="/assets/colores secundarios.png" width="300"/>

Los colores de la paleta de estados se utilizarán para los mensajes mostrados en la aplicación. El color gris oscuro (#8A8A8A) se utilizará para algunos textos informativos. Los demás colores brillantes (#7EEA91, #EEB056, #FC4E4E) se usarán para mostrar alertas según las acciones realizadas por el usuario.
<img src="/assets/paletaestados.png" width="300"/>

Las paletas de colores neutros se usarán para los textos en la aplicación. El color negro se empleará en las páginas de fondo claro, mientras que el blanco sobre los fondos de color llamativo. Los colores grises se emplearán dependiendo del énfasis que se desee dar al contenido.
<img src="/assets/coloresneutros.png" width="300"/>

**Typography:**

Como fuente para los títulos se utilizará Secular One, la cual es una fuente que destaca por su simpleza. Al ser sans-serif, también tiene un aspecto limpio y es legible aún con un tamaño pequeño.
<img src="/assets/tipografia.png" width="300"/>

Para el contenido, se utilizará la fuente Arvo que, al contrario de Secular One, es una fuente serif con aspecto más formal. Se caracteriza por su alta legibilidad en distintos pesos y tamaños, por lo que es apropiada para párrafos extensos, como pueden ser  las recetas dentro de la aplicación.
<img src="/assets/tipografiabody.png" width="300"/>
### 4.1.2. Web Style Guidelines

## 4.2. Information Architecture

### 4.2.1. Organization Systems

### 4.2.2. Labeling Systems
Navegación y menús:

Se consideraron las siguientes etiquetas y categorías para la barra de navegación:
<img src="/assets/navegacionmenus.png" width="300"/>

Contenido y Datos:

Se pueden observar etiquetas e iconos para los campos de entrada de datos:
<img src="/assets/etiquetas.png" width="300"/>
También, se incluyen etiquetas sobre las acciones que realizan los botones:
<img src="/assets/botones.png" width="300"/>


### 4.2.3. SEO Tags and Meta Tags

### 4.2.4. Searching Systems

### 4.2.5. Navigation Systems

## 4.3. Landing Page UI Design

En esta sección, se mostrará el wireframe y mock-up del landing page.

### 4.3.1. Landing Page Wireframe

<img src="/assets/Wireframe%20Landing.png" width="800"/>

### 4.3.2. Landing Page Mock-up

<img src="/assets/MockUp%20Landing.png" width="800"/>

## 4.4. Web Applications UX/UI Design

En esta sección, se mostrará los wireframes, mock-ups, wireflows y user flow diagrams de la aplicación web. Además, el prototipo de su funcionamiento.

### 4.4.1. Web Applications Wireframes

<img src="/assets/Wireframe%20Account.png" width="800"/>
<img src="/assets/Wireframe%20Sign%20In.png" width="800"/>
<img src="/assets/Wireframe%20Sign%20In%20Correct.png" width="800"/>
<img src="/assets/Wireframe%20Log%20In.png" width="800"/>

### 4.4.2. Web Applications Wireflow Diagrams

User Goal: Crear una nueva cuenta e iniciar sesión.

<img src="/assets/Wireflow%20Register.png" width="800"/>

### 4.4.3. Web Applications Mock-ups

<img src="/assets/MockUp%20Account.png" width="800"/>
<img src="/assets/MockUp%20Sign%20In.png" width="800"/>
<img src="/assets/MockUp%20Sign%20In%20Correct.png" width="800"/>
<img src="/assets/MockUp%20Log%20In.png" width="800"/>

### 4.4.4. Web Applications User Flow Diagrams

User Goal: Crear una nueva cuenta e iniciar sesión correctamente.

<img src="/assets/User%20flow%20Register.png" width="800"/>

## 4.5. Web Applications Prototyping

Link del video: 
Link del prototipo: 

## 4.6. Domain-Driven Software Architecture

### 4.6.1. Software Architecture Context Diagram

<img src="/assets/Contextdiagram.jpeg" width="800"/>

### 4.6.2. Software Architecture Container Diagrams

<img src="/assets/Container.jpeg" width="800"/>

### 4.6.3. Software Architecture Components Diagrams

<img src="/assets/Component.jpeg" width="800"/>

## 4.7. Software Object-Oriented Design

### 4.7.1. Class Diagrams

<img src="/assets/ClassDiagram.jpg" width="800"/>

### 4.7.2. Class Dictionary


## 4.8. Database Design

### 4.8.1. Database Diagram

<img src="/assets/Database.png" width="800"/>

### 4.8.2. Database Dictionary

#### User

| Campo | Tipo de Dato | Descripción |
|-|-|-|
| Usuario_ID | int | Identificador del usuario. |
| First_name | TEXT | Primer nombre del usuario. |
| Last_name | TEXT | Apellido del usuario. |
| address | TEXT | Dirección del usuario. |
| password | VARCHAR | Contraseña del usuario. |
| email | VARCHAR | Correo electrónico del usuario. |

#### Chef
| Campo | Tipo de Dato | Descripción |
|-|-|-|
| Chef_ID | int | Identificador del cocinero. |
| First_name | TEXT | Primer nombre del cocinero. |
| Last_name | TEXT | Apellido del cocinero. |
| address | TEXT | Dirección del cocinero. |
| password | VARCHAR | Contraseña del cocinero. |
| email | VARCHAR | Correo electrónico del cocinero. |

#### Menu
| Campo | Tipo de Dato | Descripción |
|-|-|-|
| Chef_ID | int | Llave Foranea - Identificador del chef al que le pertenece el menú. |
| menu_id | INT | Identificador del Menú. |
| menu_name | VARCHAR | Nombre del Menú. |
| Menu_description | TEXT | Descripción del Menú. |

#### Order
| Campo | Tipo de Dato | Descripción |
|-|-|-|
| id_ order | int | Identificador de la orden. |
| Customer_ID | int | Llave Foranea - Identificador del cliente que realizó la orden. |
| Chef_ID | int | Llave Foranea - Identificador del cocinero que recibió la orden. |
| total-orders_id | INT | Llave Foranea - Identificador del voucher al que pertenece la orden. |
| item_name | VARCHAR | Nombre del item que se ordenó. |
| price | DECIMAL | Precio de la orden. |
| address | TEXT | Dirección a la que va dirigida la orden. |

#### Order-Details
| Campo | Tipo de Dato | Descripción |
|-|-|-|
| id_order | int | Llave Foranea - Identificador de la orden a la que pertenecen los detalles. |
| order_detail_id | INT | Identificador de los detalles de orden. |
| shipping_time | TIME | Hora programada por el cliente para la realización del pedido. |
| UnitPrice | DECIMAL | Precio unitario. |
| Quantity | INT | Cantidad |

#### Dish
| Campo | Tipo de Dato | Descripción |
|-|-|-|
| dish_id | int | Identificador del platillo. |
| dish_name | TEXT | Nombre del platillo. |
| Category_ID | int | Llave Foranea - Identificador de la categoría del platillo. | 
| Cod_inform_nutri_ID | INT | Llave Foranea - Identificador de la información nutricional. |

#### Publication
| Campo | Tipo de Dato | Descripción |
|-|-|-|
| public_ID | INT | Identificador de la publicación. |
| Chef_ID | INT | Llave Foranea - Identificador del cocinero que hizo la publicación. |
| public_date | DATE | Fecha en la que se realizó la publicación. |
| title_public | TEXT | Título de la publicación. |
| descripcion | TEXT | Descripción de la publicación. |

#### Reviews
| Campo | Tipo de Dato | Descripción |
|-|-|-|
| review_id | INT | Identificador de la reseña. |
| Customer_ID | INT | Llave Foranea - Identificador del cliente que realizó la reseña. |
| Chef_ID | INT | Llave Foranea - Identificador del Cocinero que recibe la reseña. |
| review_day | DATE | Día de la reseña. |
| Comments | TEXT | Comentarios de la reseña. |
| Points | INT(5) | Puntos de la reseña. |

#### Category
| Campo | Tipo de Dato | Descripción |
|-|-|-|
| menu_id | INT | Llave Foranea - Identificador del menú. |
| Category_ID | INT | Identificador de la categoría. |
| Category_name | VARCHAR | Nombre de la categoría. |

#### Plans-Type
| Campo | Tipo de Dato | Descripción |
|-|-|-|
| plan_id | INT | Identificador del plan. |
| plan_name | TEXT | Nombre del plan. |
| price | DECIMAL | Precio del plan. |