---
title: Introdución
description: Vale docs
layout: ../../layouts/MainLayout.astro
---

Vale es una pequeña libreria para la validacion de formularios
e inputs, la cual incluye validaciones basicas como:

- ✅ **Validacion de formularios vacios**
- ✅ **Validaciones de inputs iguales**
- ✅ **Validacion de inputs individuales**
- ✅ **Validaciones concatenando funciones**
- ✅ **Armar tus propias validaciones**
- ✅ **Validacion de simbolos**
- ✅ **Manejo de mensaje de errores**

## Inicio rapido

Para comenzar a usar vale, solo debes importar la libreria y crear una instancia de la misma.

```js
import { validator } from './validator.js';
```

## Validacion de formularios vacios

Para validar un formulario vacio, solo debes pasarle un objeto con los inputs que quieres validar, y una funcion que se ejecutara si el formulario esta vacio.

```js
const z = new validator();
const inputs = document.querySelectorAll('input');
z.form().isFormEmpty(inputs);
if (z.error) {
	alert(z.error);
}
```

Suerte valiente aventurero, espero que esta libreria te sea de utilidad. 🤞
