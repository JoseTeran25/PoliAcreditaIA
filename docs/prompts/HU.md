---
title: "HU — Prompt"
date: "2025-09-30T17:09:14.259Z"
layout: default
hu: "HU"
id: "HU"
---

output: |
  ## Descripción de la Historia de Usuario HU5087

  Como usuario de Poliacredita, quiero iniciar sesión en el sistema para acceder a mis funcionalidades y datos personales de manera segura.

  ### Criterios de Aceptación
  - El sistema debe permitir al usuario ingresar su nombre de usuario y contraseña para iniciar sesión.
  - Las contraseñas deben ser almacenadas de forma segura utilizando hashing.
  - Al iniciar sesión correctamente, el sistema debe generar y devolver un token de autenticación (JWT) que permita al usuario acceder a recursos protegidos.
  - Si las credenciales son incorrectas, el sistema debe informar al usuario y no permitir el acceso.
  - El sistema debe validar el rol del usuario seleccionado para asegurarse de que tenga los permisos adecuados para iniciar sesión.

  ### Tareas Técnicas
  - [5122] Implementar el hashing de contraseñas para asegurar que las contraseñas almacenadas en la base de datos no sean legibles.
  - [5124] Generar y gestionar tokens de autenticación (JWT) para permitir sesiones seguras y mantener el estado del usuario autenticado.
  - [5126] Implementar la lógica de validación de credenciales, asegurando que se verifiquen correctamente el nombre de usuario y la contraseña.
  - [5133] Crear el endpoint `POST /auth/login` para que los usuarios puedan enviar sus credenciales y recibir un token de autenticación en respuesta.
  - [5136] Validar el rol seleccionado para autenticación, asegurando que el usuario tenga los permisos necesarios para acceder al sistema.
