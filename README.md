# CRM System - Frontend

> Sistema CRM profesional construido con React 19, TypeScript, Vite y Tailwind CSS

[![React](https://img.shields.io/badge/React-19.2-blue.svg)](https://react.dev)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.9-blue.svg)](https://www.typescriptlang.org)
[![Vite](https://img.shields.io/badge/Vite-7.2-purple.svg)](https://vitejs.dev)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind-3.4-cyan.svg)](https://tailwindcss.com)

## Inicio Rápido (3 pasos)

```bash
# 1. Instalar dependencias
npm install

# 2. Configurar variables de entorno
cp .env.example .env

# 3. Iniciar el proyecto
npm run dev
```

**¡Listo!** El proyecto se abrirá en [http://localhost:3000](http://localhost:3000)

## ✨ Características

-  **Vite** - Build tool ultra rápido con HMR
-  **React 19** - Última versión de React
-  **TypeScript** - Tipado estático para mayor seguridad
-  **Tailwind CSS** - Estilos utilitarios configurados
-  **Autenticación** - Sistema completo con Context API
-  **Dashboard** - Panel con métricas y estadísticas
-  **Gestión de Clientes** - CRUD completo
-  **Leads & Tasks** - Seguimiento y gestión
-  **Componentes** - 9 componentes reutilizables
-  **Custom Hooks** - Lógica compartida
-  **Servicios API** - Cliente HTTP modular
-  **TypeScript** - Tipos definidos
-  **Utilidades** - Format, Validation, Helpers

## ��� Estructura del Proyecto

```
src/
├── components/          # Componentes reutilizables
│   ├── common/         # Button, Input, Card, Modal, Spinner
│   └── layout/         # Header, Sidebar, MainLayout
├── pages/              # Dashboard, Customers, Login
├── services/           # API, Auth, Customer services
├── hooks/              # useAuth, useFetch, useLocalStorage
├── context/            # AuthContext
├── types/              # TypeScript interfaces
├── utils/              # Format, Validation, Helpers
└── config/             # Constants, Environment
```

## Componentes Disponibles

### Componentes Comunes
- **Button** - 4 variantes con loading state
- **Input** - Con validación y mensajes de error
- **Card** - Contenedor con título y footer
- **Modal** - Responsive con backdrop
- **Spinner** - Indicador de carga (3 tamaños)

### Layout
- **MainLayout** - Layout completo con sidebar y header
- **Header** - Barra superior con info de usuario
- **Sidebar** - Navegación lateral

## Servicios API

```typescript
// Autenticación
await authService.login({ email, password });
await authService.logout();

// Clientes
await customerService.getAll({ page: 1, limit: 10 });
await customerService.create(data);
await customerService.update(id, data);
await customerService.delete(id);
```

## Custom Hooks

```typescript
// Hook de autenticación
const { user, isAuthenticated, login, logout } = useAuth();

// Hook para fetch con estados
const { data, loading, error, refetch } = useFetch(fetchFn);

// Hook para localStorage reactivo
const [value, setValue] = useLocalStorage('key', initialValue);
```

## Scripts Disponibles

```bash
npm run dev       # Desarrollo (puerto 3000)
npm run build     # Compilar para producción
npm run preview   # Preview del build
npm run lint      # Ejecutar ESLint
```

## Documentación

- **[INSTALL.md](INSTALL.md)** - Guía completa de instalación
- **[QUICKSTART.md](QUICKSTART.md)** - Inicio rápido de 5 minutos
- **[DOCS.md](DOCS.md)** - Documentación completa de API
- **[EXAMPLES.md](EXAMPLES.md)** - 7 ejemplos prácticos con código
- **[ARCHITECTURE.md](ARCHITECTURE.md)** - Arquitectura del sistema
- **[STRUCTURE.md](STRUCTURE.md)** - Resumen de archivos creados

## Variables de Entorno

```env
VITE_API_BASE_URL=http://localhost:3000/api
```

## Tecnologías

- **Frontend**: React 19.2, TypeScript 5.9
- **Build Tool**: Vite 7.2
- **Estilos**: Tailwind CSS 3.4
- **Estado**: Context API + Custom Hooks
- **HTTP Client**: Fetch API con servicio wrapper
- **Validación**: Utilidades personalizadas
- **Formateo**: Intl API

## Dependencias Principales

```json
{
  "react": "^19.2.0",
  "react-dom": "^19.2.0",
  "typescript": "~5.9.3",
  "vite": "^7.2.4",
  "tailwindcss": "^3.4.17"
}
```

## Configuración

### Path Aliases
El proyecto usa \`@/\` para imports absolutos:

```typescript
import { Button } from '@/components/common';
import { apiService } from '@/services';
import type { User } from '@/types';
```

## ��� Características Implementadas

✅ Sistema de autenticación completo  
✅ Gestión de clientes (CRUD)  
✅ Dashboard con métricas  
✅ Componentes reutilizables  
✅ Custom hooks  
✅ Servicios API modulares  
✅ Utilidades (format, validation, helpers)  
✅ TypeScript estricto  
✅ Path aliases (@/)  
✅ Tailwind CSS configurado  
✅ Responsive design ready  

## Próximos Pasos

Ver **[INSTALL.md](INSTALL.md)** para dependencias opcionales recomendadas.

## Ejemplo de Uso

```tsx
import { Button, Card } from '@/components/common';
import { useAuth } from '@/hooks';

function MyComponent() {
  const { user } = useAuth();

  return (
    <Card title="Mi Componente">
      <Button>Guardar</Button>
    </Card>
  );
}
```

---

**¿Necesitas ayuda?** Revisa la documentación en los archivos \`.md\`

**¡Happy Coding!** ���

<img width="1904" height="942" alt="image" src="https://github.com/user-attachments/assets/30c3bd43-39e7-4bde-b59c-14bbbb39a9d8" />
<img width="1918" height="940" alt="image" src="https://github.com/user-attachments/assets/73d8fdda-51e7-4fa2-abf5-56392e0df238" />



