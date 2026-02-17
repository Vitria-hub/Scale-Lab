# Flujo para crear una Landing Page

Este documento describe la información necesaria para encargar una landing page al equipo de desarrollo.

---

## Lo que debes recolectar del cliente

### 1. URL del sitio web
Pasa la URL del sitio del cliente. Se usa para analizar marca, colores, tipografía y tono visual de forma automática.

---

### 2. Brief del cliente

**Sobre la marca**
- ¿Qué venden y por qué nació la marca?
- ¿Qué los hace distintos a la competencia?
- ¿Quiénes son sus competidores directos?

**Cliente ideal**
- ¿Quién es su cliente perfecto? (edad, género, ciudad, estilo de vida)
- ¿Qué problema o dolor resuelven?
- ¿Qué cambio espera vivir al usar el producto? (funcional y emocional)
- ¿Dónde usan el producto?
- ¿Quién lo compra? ¿Es para sí mismo o para regalar?

**Confianza y objeciones**
- ¿Qué duda tienen antes de comprar?
- ¿Qué prueba social tienen? (reseñas, influencers, UGC, prensa)
- ¿Qué emoción principal quieren transmitir?

**Producto y oferta**
- ¿Cuál es el producto estrella a impulsar? (nombre + beneficios)
- ¿Tienen oferta o promesa clave? (descuento, garantía, envío gratis, etc.)
- ¿Qué frases usan sus clientes al hablar del producto?

---

### 3. URLs de los productos a mostrar
Links directos de Shopify (u otra tienda) de cada producto que aparecerá en la landing. Se extraen precios, imágenes y descripciones automáticamente.

---

### 4. Nombre del proyecto
Nombre corto del cliente en minúsculas y sin espacios. Ejemplos: `mindset`, `one-chile`, `nombre-marca`.
Se usa para nombrar la carpeta en el repo y el proyecto en Vercel.

---

## Lo que pasa después (automático)

1. Se analiza el sitio web → se extraen colores, tipografía y tono visual
2. Se construye la landing con estructura **Listicle CRO** (metodología Carl Weische)
3. Se sacan imágenes reales del CDN del cliente (sin placeholders)
4. Push a GitHub → `Vitria-hub/Scale-Lab/nombre-cliente-landing/`
5. Se crea proyecto nuevo en Vercel con su propia URL

**Tiempo desde que se entrega la info completa: ~15 minutos.**

---

## Estructura del repo

```
Scale-Lab/
├── one-chile-landing/     → scale-lab.vercel.app
├── mindset-landing/       → scale-lab-qp6e.vercel.app
└── nuevo-cliente-landing/ → URL nueva por cliente
```

Cada cliente tiene su carpeta y su propio proyecto en Vercel. Un push al repo actualiza solo el proyecto correspondiente.
