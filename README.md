# Hola, soy Jairo 👋

Estudiante de Ingeniería de Sistemas en la Javeriana (Bogotá). Me interesa que el software **funcione bien de verdad**, no solo en el caso feliz: probarlo, medirlo y encontrar dónde falla antes que el usuario.

---

## 🏥 MEDIX · proyecto de grado (Mención de Honor)

Asistente para agendar citas médicas **hablando**, pensado para personas a las que les cuesta usar apps. El paciente dice *"quiero una cita con medicina general o alguna especialidad"* y el sistema entiende, consulta la agenda de la IPS y la reserva.

```mermaid
flowchart LR
    APP["📱 App Android<br/>Kotlin"] -- "texto / voz" --> AI["🤖 IA conversacional<br/>FastAPI · Whisper"]
    AI --> API["📅 API de citas<br/>FastAPI · Supabase"]
    APP --> API
    ADMIN["🖥️ Portal admin<br/>Next.js"] --> API
    API -- "HL7 FHIR R4" --> IPS["🏥 IPS simulada"]
    REM["🔔 Recordatorios<br/>Node · Twilio · Firebase"] --> APP
```

| Servicio | Qué hace |
|---|---|
| [medix-app](https://github.com/G11-Medix/medix-app) | App Android: registro, citas, consentimiento y asistente por texto o voz |
| [medix-ai-api](https://github.com/G11-Medix/medix-ai-api) | Reconocimiento de voz con Whisper, manejo de la conversación y extracción de datos de la cita |
| [medix-appointments-api](https://github.com/G11-Medix/medix-appointments-api) | API REST de pacientes, citas y catálogos, con auditoría de operaciones |
| [ips-mock-service](https://github.com/G11-Medix/ips-mock-service) | Simula los sistemas de agenda de las IPS con el estándar **HL7 FHIR R4** |
| [portal-admin-medix](https://github.com/G11-Medix/portal-admin-medix) | Portal web para supervisar pacientes, citas e integraciones |
| [medix-reminders-service](https://github.com/G11-Medix/medix-reminders-service) | Recordatorios de citas por SMS y notificaciones push |

El proyecto incluye pruebas funcionales con pytest y colecciones de Bruno, **pruebas de carga** y mediciones de latencia del reconocimiento de voz y de precisión de la IA.

---

## 🧪 QA Automation Portfolio

[**qa-automation-portfolio**](https://github.com/Jairo-Andres/qa-automation-portfolio) · Pruebas E2E de una tienda online con **Playwright** y pruebas de una API REST con **Postman**, que se ejecutan solas en cada push con GitHub Actions.

Lo más interesante fue lo que no estaba planeado: la API tenía [bugs reales que documenté](https://github.com/Jairo-Andres/qa-automation-portfolio/blob/main/docs/BUGS.md), y un fallo intermitente en CI resultó ser el servidor reiniciándose en mitad de las pruebas.

---

## 📊 Datos

La otra mitad de lo que me interesa: convertir datos en decisiones. Hice el énfasis de la carrera en **bases de datos y visualización**, y lo aplico en lo que construyo:

- En **MEDIX**, medir la latencia del reconocimiento de voz y evaluar la IA con una matriz de confusión fue lo que nos dijo qué mejorar, más allá de "parece que funciona".
- En el **[Semillero de Producción y Logística](https://github.com/Jairo-Andres/Semillero)** desarrollé la lógica de programación de la producción y analicé los resultados para apoyar decisiones de planta.

Herramientas: Python (pandas), R, Power BI y SQL.

---

## 🛠️ Con qué trabajo

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat&logo=fastapi&logoColor=white)
![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=flat&logo=kotlin&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat&logo=openjdk&logoColor=white)
![Playwright](https://img.shields.io/badge/Playwright-2EAD33?style=flat)
![Pytest](https://img.shields.io/badge/pytest-0A9EDC?style=flat&logo=pytest&logoColor=white)
![Postman](https://img.shields.io/badge/Postman-FF6C37?style=flat&logo=postman&logoColor=white)
![Bruno](https://img.shields.io/badge/Bruno-F4AA41?style=flat&logo=bruno&logoColor=black)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat&logo=mysql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat&logo=mongodb&logoColor=white)
![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=flat&logoColor=black)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white)

---

📫 Hablemos en [LinkedIn](https://www.linkedin.com/in/jairo-andres31-analyst/)
