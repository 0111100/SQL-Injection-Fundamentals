## Introduction 

1. **Introducción a la Estructura de Bases de Datos en Aplicaciones Web**: 

  - Las aplicaciones web modernas utilizan bases de datos para almacenar y recuperar datos, lo que permite la entrega de contenido dinámico. Las solicitudes HTTP(S) desencadenan interacciones entre el backend de la aplicación web y la base de datos para construir respuestas.

![image](https://github.com/0111100/SQL-Injection-Fundamentals/assets/96475451/8a0f00f3-8e95-4ac1-826f-04fd0da30de1)


2. **Inyección de SQL (SQLi)**:   

   - Definición: La inyección de SQL ocurre cuando usuarios malintencionados manipulan la entrada para alterar las consultas SQL enviadas por la aplicación web a la base de datos.
   - Objetivo: Los atacantes buscan ejecutar consultas no deseadas, potencialmente accediendo a datos sensibles o subvirtiendo la lógica de la aplicación.
   - Técnicas: Inyección de código SQL, como comillas simples (' o "), para eludir las restricciones de entrada, seguida de la ejecución de consultas maliciosas mediante técnicas como consultas apiladas o consultas de unión.

3. **Casos de Uso e Impacto**:
   
   - Recuperación de Información: Los atacantes pueden acceder a datos sensibles como credenciales de usuario o información de tarjetas de crédito, lo que lleva a brechas y un posterior uso indebido.
   - Subversión de la Lógica de la Aplicación: La inyección de SQL puede eludir mecanismos de autenticación, acceder a funciones restringidas e incluso comprometer la integridad del servidor mediante la lectura o escritura de archivos y el establecimiento de puertas traseras.

4. **Prevención**:
   
   - Prácticas de Codificación Segura: Implementar técnicas robustas de saneamiento y validación de entradas para prevenir la manipulación de entradas malintencionadas.
   - Seguridad en el Backend: Mantener un estricto control sobre los privilegios del servidor y la base de datos para limitar las superficies de ataque potenciales.

Al comprender los mecanismos de la inyección de SQL y adoptar medidas preventivas, los desarrolladores pueden fortalecer las aplicaciones web contra esta vulnerabilidad común y potencialmente devastadora.


## Architecture


![image](https://github.com/0111100/SQL-Injection-Fundamentals/assets/96475451/c5d0ceb5-a4a1-472d-b003-46c3ffe57e48)


| **Feature**                 | **Description**                                                                                                                                                                            |
| --------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `Concurrency`               | A real-world application might have multiple users interacting with it simultaneously. A DBMS makes sure that these concurrent interactions succeed without corrupting or losing any data. |
| `Consistency`               | With so many concurrent interactions, the DBMS needs to ensure that the data remains consistent and valid throughout the database.                                                         |
| `Security`                  | DBMS provides fine-grained security controls through user authentication and permissions. This will prevent unauthorized viewing or editing of sensitive data.                             |
| `Reliability`               | It is easy to backup databases and rolls them back to a previous state in case of data loss or a breach.                                                                                   |
| `Structured Query Language` | SQL simplifies user interaction with the database with an intuitive syntax supporting various operations.                                                                                  |

