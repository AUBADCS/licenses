# Auba DCS — Servidor de Licencias (Nube)

Repositorio público en la nube para la validación distribuida y segura de licencias de las extensiones de **Auba DCS** en Microsoft Dynamics 365 Business Central.

---

## 🔒 Seguridad y Privacidad
- **Contenido Cifrado:** El archivo `licenses.json` alojado en este repositorio contiene exclusivamente información cifrada mediante **AES-256 / XOR** con clave simétrica.
- **Acceso Público de Lectura:** Al estar encriptado, el archivo es seguro para la lectura pública y permite que los entornos de Business Central de los clientes verifiquen su estado sin necesidad de gestionar credenciales o tokens individuales.
- **Escritura Restringida:** Solo la aplicación central de Auba DCS (`Auba Control Licencias`) cuenta con permisos de modificación mediante un token de acceso personal (PAT) de la organización `AUBADCS`.

---

## 📄 Estructura del Servidor
- `licenses.json`: Payload cifrado actualizado en tiempo real por el Business Central interno de Auba DCS.
