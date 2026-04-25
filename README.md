# 💳 Tarjeta de Presentación – Bayron Flores

Diseño moderno y minimalista de tarjeta de presentación para desarrollador Full Stack, con estilo oscuro y acentos en tonos verdes/menta. Ideal para uso digital o impresión.

---

## 🖼️ Vista previa

### 🔹 Cara Frontal

![Frontal](assets/frontal.png)

### 🔹 Cara Trasera

![Trasera](assets/trasera.png)

> 📌 Puedes reemplazar estas imágenes en la carpeta `/assets` con capturas reales del diseño.

---

## 🎨 Características del diseño

- Estilo moderno y profesional
- Diseño doble cara (front/back)
- Uso de SVG para gráficos dinámicos
- Paleta de colores tecnológica (verde oscuro + menta)
- Tipografía clara y jerarquizada
- Adaptado para:
  - 💻 Uso digital (portafolio)
  - 🖨️ Impresión física

---

## 🧩 Tecnologías utilizadas

- **HTML5**
- **CSS3** (Flexbox + diseño responsive)
- **SVG** (gráficos vectoriales)
- **JavaScript** (generación dinámica de contenido)

---

## 📐 Dimensiones

| Propiedad | Valor                       |
| --------- | --------------------------- |
| Tamaño    | 356px × 200px               |
| Relación  | Tarjeta estándar horizontal |

---

## 🎯 Contenido de la tarjeta

### Frontal

- Nombre completo
- Rol profesional
- Stack tecnológico
- Información de contacto:
  - 📧 Email
  - 📞 Teléfono
  - 📍 Ubicación

### Trasera

- Nombre destacado
- Frase profesional
- Usuario de GitHub

---

## 🎨 Paleta de colores

| Color         | Código    | Uso                    |
| ------------- | --------- | ---------------------- |
| Fondo oscuro  | `#161614` | Base frontal           |
| Verde         | `#0F6E56` | Elementos principales  |
| Verde oscuro  | `#085041` | Fondo trasero          |
| Menta         | `#9FE1CB` | Acentos                |
| Verde claro   | `#E1F5EE` | Información secundaria |
| Acento nombre | `#5DCAA5` | Apellido               |

---

## 📂 Estructura del proyecto

```
📁 tarjeta-de-presentacion/
│
├── Diseño-Tarjeta.html       ← Estructura y lógica visual
├── card-data.js              ← ⚠️ NO incluido en el repositorio (ver abajo)
├── card-data.example.js      ← Plantilla de referencia para crear card-data.js
├── .gitignore
├── README.md
└── assets/
    ├── frontal.png
    └── trasera.png
```

---

## 🔐 Configuración de datos personales (`card-data.js`)

Los datos personales de la tarjeta (nombre, email, teléfono, etc.) se gestionan en un archivo separado llamado **`card-data.js`**, el cual **no se sube al repositorio** por contener información sensible.

### Pasos para configurarlo

1. Copia el archivo de ejemplo incluido en el proyecto:

```bash
cp card-data.example.js card-data.js
```

2. Abre `card-data.js` y completa tus datos:

```js
const CARD = {
  /* ── Identidad ── */
  nameFirst: "Tu Nombre",
  nameLast: "Tu Apellido",

  /* ── Cara frontal ── */
  tag: "Tu título profesional", // ej: "Ing. Informática · Full Stack Dev"
  role: "Tu rol", // ej: "Desarrollador Web & Móvil"
  stack: ["Tech1", "Tech2", "Tech3"], // tecnologías que aparecen como pills

  /* ── Contacto ── */
  email: "tuemail@ejemplo.com",
  phone: "+56 9 0000 0000",
  location: "Ciudad, País",

  /* ── Cara trasera ── */
  tagline: "Línea 1\nLínea 2", // \n genera un salto de línea
  github: "github.com/TuUsuario",

  qrUrl: "https://tuportafolio.com", // URL que codifica el QR
};
```

> ⚠️ `card-data.js` está listado en `.gitignore` y **nunca debe subirse al repositorio**.  
> Comparte tus datos solo con quienes deban tenerlos, de forma privada.

---

## 🚀 Cómo usar

1. **Clona el repositorio:**

```bash
git clone https://github.com/BayronFlores/tarjeta-de-presentacion.git
```

2. **Crea tu archivo de datos** siguiendo las instrucciones de la sección anterior.

3. **Abre el archivo con un servidor local** (ej: [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) en VS Code):

> ⚠️ No abras `Diseño-Tarjeta.html` directamente con doble clic. Los navegadores bloquean la carga de scripts externos en protocolo `file://`. Usa un servidor local para que `card-data.js` se cargue correctamente.

---
