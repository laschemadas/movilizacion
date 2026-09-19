# Caja de herramientas · Medellín se comunica aprendiendo

Producto mínimo viable (MVP) de la **Caja de herramientas para la comunicación
comunitaria, alternativa, independiente y ciudadana** de la Secretaría de
Comunicaciones del Distrito de Ciencia, Tecnología e Innovación de Medellín.

Es un sitio estático: una portada (`index.html`) que reúne y enlaza todas las
piezas interactivas construidas hasta hoy, para verlas juntas, en línea y
navegables. No necesita servidor ni base de datos.

## Qué incluye

La portada agrupa 14 piezas en cuatro secciones:

**Empieza aquí**
- Medellín se comunica aprendiendo — portada formativa (planeador, cartas de acción, 5C)
- Caja de herramientas · Módulos — índice de la ruta pedagógica

**Formación (serious games)**
- Ley 1712 · Detective de datos — transparencia y acceso a la información
- Ley 1755 · El caso — derecho de petición
- MIPG · Dirige tu dependencia — gestión pública
- Participación · La escalera de la incidencia — Ley 1757
- Sala de Medios — decisiones de un medio ciudadano

**Guías y estándares**
- Guía de Lenguaje Claro
- Estándar técnico de publicación digital v2
- Anexo 8 · Accesibilidad digital

**Tableros y utilidades**
- Tablero Participa Medellín
- Verificador de contraste
- Demo · Diagnóstico de Accesibilidad
- Respuestas de Chat en Vivo

## Estructura

```
.
├── index.html            # Portada / lanzador del MVP
├── piezas/               # Cada herramienta como HTML autónomo
│   ├── hub-medellin-comunica.html
│   ├── modulos.html
│   └── ... (14 piezas en total)
├── vercel.json           # Cabeceras de seguridad (opcional)
├── .gitignore
└── README.md
```

Cada archivo en `piezas/` es una página HTML autocontenida (CSS y JS embebidos).
Los enlaces entre piezas son relativos, así que el sitio funciona igual en local,
en GitHub Pages o en Vercel.

## Ver en local

Abre `index.html` en el navegador, o levanta un servidor simple:

```bash
python3 -m http.server 8000
# luego abre http://localhost:8000
```

## Accesibilidad

La portada usa la paleta AAA del Anexo 8 del Manual de Identidad Visual de la
Alcaldía. Contraste verificado por script: 23 de 23 pares alcanzan WCAG AAA en
tema claro y oscuro. Pendiente la validación con lectores de pantalla y personas
usuarias antes de una declaración formal de conformidad.

## Marco normativo de referencia

Constitución Política de Colombia · Ley 1712 de 2014 (transparencia) · Ley 1755
de 2015 (derecho de petición) · Ley 1757 de 2015 (participación) · MIPG · Anexo 8
del Manual de Identidad Visual de la Alcaldía de Medellín.

---

Secretaría de Comunicaciones · Distrito de Ciencia, Tecnología e Innovación · Medellín
