# ⏱ CountlyHours

**Controlá tus horas. Maximizá tu dinero.**

Aplicación web para trabajadores de hostelería y restauración que registran turnos en múltiples ETTs y quieren saber exactamente cuánto ganan, separando horas diurnas y nocturnas según convenio.

---

## 🚀 Demo

> Abrí `countlyhours-v3.1.html` en tu navegador local o deployá en Netlify.

Para funcionalidad completa (login, registro, sincronización en la nube) necesitás servir el archivo desde un servidor HTTP, no desde `file://`.

```bash
# Servidor local rápido
cd carpeta-del-proyecto
python3 -m http.server 8080
# → http://localhost:8080/countlyhours-v3.1.html
```

---

## ✨ Features

| Feature | Gratis | Pro (€2,99/mes) | Business (€6,99/mes) |
|---|---|---|---|
| Registro de turnos ilimitado | ✓ | ✓ | ✓ |
| Múltiples ETTs con tarifas propias | ✓ | ✓ | ✓ |
| Dashboard mensual | ✓ | ✓ | ✓ |
| Exportar CSV | ✓ | ✓ | ✓ |
| Historial completo | — | ✓ | ✓ |
| Exportar PDF profesional | — | ✓ | ✓ |
| Comparativa de ETTs | — | ✓ | ✓ |
| Alertas de meta | — | ✓ | ✓ |
| Hasta 5 perfiles | — | — | ✓ |
| Informe mensual por email | — | — | ✓ |
| Soporte prioritario 24h | — | — | ✓ |

---

## 🛠 Stack

- **Frontend**: HTML + CSS + Vanilla JS (single file, sin frameworks)
- **Auth + DB**: [Supabase](https://supabase.com) (PostgreSQL + Auth)
- **Deploy**: [Netlify](https://netlify.com) (drag & drop o deploy automático desde Git)
- **Pagos** *(próximamente)*: [Stripe](https://stripe.com) Subscriptions

---

## ⚙️ Configuración de Supabase

1. Crear proyecto en [supabase.com](https://supabase.com)
2. Ejecutar el SQL de `supabase_setup.sql` en el SQL Editor
3. Reemplazar en el archivo HTML:
   ```js
   const _SB = supabase.createClient('TU_URL', 'TU_ANON_KEY');
   ```
4. Activar Google OAuth en **Authentication → Providers → Google**

---

## 📦 Estructura

```
countlyhours/
├── countlyhours-v3.1.html   # App completa (single file)
├── supabase_setup.sql        # Schema de base de datos
└── README.md
```

---

## 🗺 Roadmap

- [ ] Integración Stripe (suscripciones Pro y Business)
- [ ] Diseño responsive mobile
- [ ] PWA (installable en móvil)
- [ ] Notificaciones push para turnos pendientes
- [ ] Informe mensual automático por email (Business)

---

## 📬 Contacto

handandshake.contacto@gmail.com

---

© 2026 CountlyHours
