# Seguridad en Sistemas Embebidos
## Quiñonez Agramon Angel Gabriel / AngelAgramon / 21210860
## Introducción
Los sistemas embebidos son dispositivos con software dedicado a realizar funciones específicas. Su creciente adopción en IoT, automóviles, dispositivos médicos y sistemas industriales los convierte en objetivos de ataques cibernéticos. La seguridad en estos sistemas es fundamental para proteger datos sensibles y garantizar su funcionamiento correcto.

## Criptografía en Sistemas Embebidos
La criptografía es un mecanismo clave para proteger la información en sistemas embebidos. Existen varias técnicas utilizadas:

### Algoritmos de Cifrado
- **AES (Advanced Encryption Standard)**: Algoritmo simétrico ampliamente utilizado por su equilibrio entre seguridad y rendimiento.
- **RSA (Rivest-Shamir-Adleman)**: Algoritmo asimétrico usado para intercambio de claves y firmas digitales.
- **ECC (Elliptic Curve Cryptography)**: Alternativa eficiente a RSA con mayor seguridad para claves más pequeñas.

### Firmas Digitales
Las firmas digitales garantizan la autenticidad e integridad de los datos transmitidos. Se basan en algoritmos asimétricos como RSA o ECC y proporcionan verificación de identidad en entornos embebidos.

### Generación de Números Aleatorios
Para una criptografía segura, se requieren números aleatorios de alta calidad. Se utilizan generadores de números pseudoaleatorios (PRNG) y generadores de números aleatorios verdaderos (TRNG).

## Autenticación en Sistemas Embebidos
La autenticación es el proceso de verificar la identidad de un usuario o dispositivo. Métodos comunes incluyen:

### Autenticación Basada en Claves
- **Contraseñas y PINs**: Método básico pero susceptible a ataques de fuerza bruta.
- **Claves criptográficas**: Uso de claves compartidas o públicas para verificar identidades.

### Autenticación Basada en Hardware
- **TPM (Trusted Platform Module)**: Chip especializado que almacena claves y realiza operaciones criptográficas.
- **Secure Elements**: Circuitos diseñados para manejar datos sensibles y resistir ataques físicos.

### Autenticación de Dispositivos
- **Protocolos como OAuth y TLS**: Garantizan una comunicación segura entre dispositivos y servidores.
- **Identificación basada en huellas digitales de hardware**: Técnicas como PUFs (Physical Unclonable Functions) permiten autenticación única de cada dispositivo.

## Protección Contra Ataques
Los sistemas embebidos están expuestos a diversas amenazas, por lo que se implementan medidas para mitigar riesgos:

### Ataques Comunes y Contramedidas
- **Ataques de fuerza bruta**: Uso de contraseñas robustas y autenticación multifactor.
- **Ataques de canal lateral**: Blindaje electromagnético y técnicas de ofuscación para evitar fugas de información.
- **Ataques de inyección de código**: Uso de técnicas como DEP (Data Execution Prevention) y ASLR (Address Space Layout Randomization).
- **Ataques de hardware**: Implementación de medidas antifalsificación y detección de manipulación.

### Actualizaciones Seguras
Las actualizaciones de firmware deben ser seguras para prevenir ataques:
- **Verificación de firma digital** en actualizaciones.
- **Canales cifrados** para la distribución del firmware.
- **Rollback protection** para evitar el uso de versiones vulnerables anteriores.

## Conclusión
La seguridad en sistemas embebidos es un desafío crítico que requiere el uso de criptografía avanzada, autenticación robusta y protección contra ataques físicos y lógicos. La implementación de buenas prácticas y tecnologías adecuadas es esencial para mitigar riesgos y garantizar la confiabilidad de estos sistemas en entornos críticos.

