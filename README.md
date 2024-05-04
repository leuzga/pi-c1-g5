# React + TypeScript + Vite

#### Proyecto PI_C1_G5

El acronimo significa proyecto integrador camada1 grupo 5
el presente proyecto es un init template puede ser descargado o clonado como template incio

Estandarización del Desarrollo React para el Proyecto: Guía Completa
--------------------------------------------------------------------

## Atención

> El presente texto es una aproximacion del proyecto
> se aceptan todo tipo de sugerencias ya que es un proyecto colaborativo en equipo
> este documento formará parte de la documentacion del proyecto actual

# Estandarización del Desarrollo React para el Proyecto: Guía Detallada

## Introducción

El proyecto React requiere un enfoque estandarizado para garantizar la coherencia, la eficiencia y la colaboración entre los miembros del equipo. Este documento establece las herramientas y prácticas recomendadas para el desarrollo, la gestión de tareas, el diseño, la comunicación y la implementación.

## Gestión de Tareas

| Herramienta | Descripción | Enlace |
| --- | --- | --- |
| Taiga | Herramienta de gestión de proyectos ágil y flexible que permite la creación de tableros Kanban, sprints, tareas y subtareas, la asignación de responsabilidades y el seguimiento del progreso. | <https://taiga.io/> |
| Trello | Alternativa popular a Taiga que ofrece una interfaz visual intuitiva para organizar tareas, priorizar el trabajo y colaborar en equipo. | <https://trello.com/> |

## Diseño

| Herramienta | Descripción | Enlace |
| --- | --- | --- |
| Figma | Herramienta de diseño de interfaz de usuario basada en la nube que permite crear prototipos interactivos, compartir diseños con el equipo y obtener comentarios en tiempo real. | <https://www.figma.com/> |

## Comunicación

| Herramienta | Descripción | Enlace |
| --- | --- | --- |
| Slack | Plataforma de comunicación en equipo popular que facilita la mensajería instantánea, las llamadas de voz y video, y la colaboración en archivos. | <https://slack.com/> |
| Discord | Alternativa a Slack con enfoque en comunidades y grupos, ofreciendo canales de chat, llamadas de voz y video, y bots para automatizar tareas. | <https://discord.com/> |

## Desarrollo

| Herramienta | Descripción | Enlace |
| --- | --- | --- |
| Visual Studio Code | Editor de código popular con extensiones para JavaScript, TypeScript, React y otras tecnologías. | <https://code.visualstudio.com/> |
| Node.js | Entorno de ejecución de JavaScript que permite ejecutar código JavaScript fuera del navegador. | <https://nodejs.org/en> |
| Vite | Herramienta de empaquetado y desarrollo de aplicaciones web moderna y eficiente que ofrece arranque rápido, recargas en caliente y soporte para TypeScript. | <https://vitejs.dev/> |
| Vitest | Marco de pruebas unitarias y de integración basado en Jest, optimizado para Vite. | <https://vitest.dev/> |

## Dependencias

| Dependencia | Descripción | Enlace |
| --- | --- | --- |
| PreactSignals | Librería de gestión de estado reactiva y ligera para Preact. | <https://github.com/preactjs/signals/blob/main/packages/preact/README.md> |
| chadcn/ui | CLI para crear componentes Preact rápidamente. | <https://github.com/shadcn-ui/ui> |
| Tailwind CSS | Framework CSS de bajo nivel que proporciona clases de utilidad para diseñar interfaces de usuario personalizadas. | <https://tailwindcss.com/> |

## Enrutamiento

| Herramienta | Descripción | Enlace |
| --- | --- | --- |
| Wouter | Librería de enrutamiento moderna y flexible para aplicaciones React. | <https://github.com/molefrog/wouter> |
| React Router v6 | Librería de enrutamiento popular para aplicaciones React. | <https://github.com/topics/react-router-dom-v6> |

## Autenticación

| Herramienta | Descripción | Enlace |
| --- | --- | --- |
| Cognito | Servicio de autenticación y gestión de usuarios de Amazon Web Services (AWS) que permite implementar inicios de sesión seguros, administración de roles y control de acceso. | <https://aws.amazon.com/cognito/> |

## Consumir API

| Herramienta | Descripción | Enlace |
| --- | --- | --- |
| Fetch API | API nativa de JavaScript para realizar solicitudes HTTP. | <https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API> |

# Estandarización de Back-End
>
> Faltaria saber que se usara en el Backend

## Expanding the ESLint configuration

If you are developing a production application, we recommend updating the configuration to enable type aware lint rules:

- Configure the top-level `parserOptions` property like this:

```js
export default {
  // other rules...
  parserOptions: {
    ecmaVersion: 'latest',
    sourceType: 'module',
    project: ['./tsconfig.json', './tsconfig.node.json'],
    tsconfigRootDir: __dirname,
  },
}
```

- Replace `plugin:@typescript-eslint/recommended` to `plugin:@typescript-eslint/recommended-type-checked` or `plugin:@typescript-eslint/strict-type-checked`
- Optionally add `plugin:@typescript-eslint/stylistic-type-checked`
- Install [eslint-plugin-react](https://github.com/jsx-eslint/eslint-plugin-react) and add `plugin:react/recommended` & `plugin:react/jsx-runtime` to the `extends` list
