# ⏱ CountlyHours
**Controlá tus horas. Maximizá tu dinero.**

Aplicación web para **trabajadores de hostelería** y **profesionales de salud** que registran turnos o sesiones en múltiples empleadores y quieren saber exactamente cuánto ganan.

- 🍽️ **Hostelería** — camareros, cocineros, bartenders con múltiples ETTs
- 🏥 **Salud** — psicólogos, fisioterapeutas, nutricionistas, coaches con múltiples pacientes

---

## 🚀 Demo en vivo
**[countlyhours.es](https://countlyhours.es)**

---

## ✨ Features

| Feature | Gratis | Pro (€2,99/mes) | Business (€6,99/mes) |
|---|:---:|:---:|:---:|
| Registro de turnos/sesiones ilimitado | ✓ | ✓ | ✓ |
| Múltiples ETTs / Pacientes con tarifas propias | ✓ | ✓ | ✓ |
| Dashboard mensual | ✓ | ✓ | ✓ |
| Exportar CSV | ✓ | ✓ | ✓ |
| Historial completo | — | ✓ | ✓ |
| Exportar PDF profesional | — | ✓ | ✓ |
| Estadísticas avanzadas por ETT/Paciente | — | ✓ | ✓ |
| Metas con alertas | — | ✓ | ✓ |
| Notas por turno | — | ✓ | ✓ |
| Hasta 3 perfiles (ej. pareja) | — | — | ✓ |
| Informe mensual automático por email | — | — | ✓ |
| Soporte prioritario 24h | — | — | ✓ |

---

## 🛠 Stack

- **Frontend:** HTML + CSS + Vanilla JS (single file, sin frameworks)
- **Auth + DB:** [Supabase](https://supabase.com) (PostgreSQL + Auth)
- **Deploy:** [Netlify](https://netlify.com) (deploy automático desde Git)
- **Email:** [Resend](https://resend.com) (transaccional)
- **Pagos:** Stripe Subscriptions *(próximamente)*

---

## ⚙️ Configuración

### Supabase
1. Crear proyecto en [supabase.com](https://supabase.com)
2. Ejecutar `admin_setup.sql` en el SQL Editor
3. Activar Google OAuth en Authentication → Providers → Google
4. Configurar Site URL: `https://countlyhours.es`

### Variables en el HTML
```js
const _SB = supabase.createClient('TU_URL', 'TU_ANON_KEY');
```

---

## 📦 Estructura

```
countlyhours/
├── index.html          # App completa (single file)
├── admin_setup.sql     # Schema de base de datos
└── README.md
```

---

## 🗺 Roadmap

- [ ] Integración Stripe (Pro + Business)
- [ ] PDF exportable por mes
- [ ] Informe mensual automático por email
- [ ] PWA instalable en móvil
- [ ] Recordatorios de turno por email
- [ ] Múltiples perfiles (Business)

---

## 📬 Contacto

[handandshake.contacto@gmail.com](mailto:handandshake.contacto@gmail.com)

---

*© 2026 CountlyHours*
