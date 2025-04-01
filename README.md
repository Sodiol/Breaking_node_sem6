# ESLint
 
 ## 📌 ¿Qué es?

 Este proyecto utiliza **ESLint** para analizar el código ejemplo.

 **ESLint** es una herramienta para identificar e informar sobre patrones encontrados en el código ECMAScript/     JavaScript.

 ## 🚀 ¿Cómo instalarlo?

 Primero inicias el proyecto `npm init -y`

 Instalas **ESLint** `npm install eslint --save-dev`

 **ESLint** se configura usando `npx eslint --init`

 ## ⚙️ Configuración de ESLint

 Este proyecto está configurado con ESLint para verificar dos reglas clave:

 `no-unused-vars`: Advierte si hay variables que se han declarado pero no se usan en el código.

 `no-undef`: Muestra un error si se intenta usar una variable que no ha sido definida.

 ``{
  "extends": "eslint:recommended",
  "rules": {
    "no-unused-vars": "warn",
    "no-undef": "error"
  }
 }``

 ## 🛠️ ¿Cómo usar ESLint?

 Para analizar tu código con **ESLint** usamos

 `npx eslint nombre_del_archivo.js`

 Para corregir

 `npx eslint nombre_del_archivo.js --fix`

 ## 📝 Ejemplo básico de uso

 Usando el archivo index.js 

 `var mensaje = 'Hola, mundo!'; 
 console.log(mensaje);
 const test = someUndefinedVariable;`

 Uso el comando

 `npx eslint index.js --fix`

 Dando como resultado

  `4:7   error  'test' is assigned a value but never used  no-unused-vars
  4:14  error  'someUndefinedVariable' is not defined     no-undef
  ✖ 2 problems (2 errors, 0 warnings)`

  

