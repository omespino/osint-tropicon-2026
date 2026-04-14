# 🕵️‍♂️ Tácticas de OSINT: Lo que Internet sabe de ti (y tú no sabías) [3]

**Instructor:** Omar Espino (@omespino) | Consultor de Seguridad en Websec y Bug Bounty Hunter [4].
**Blog Personal:** omespino.com [4].
**Evento:** TropiCON 2026 (CZM/MX) [4].

> **¡ATENCIÓN!** Toda la información y herramientas incluidas en este repositorio son exclusivamente para fines educativos y profesionales [5, 6]. Ni los organizadores del evento ni el instructor son responsables del mal uso de esta información [5, 6].

---

## 1. Identidad y Huella Digital 👣
Conceptos fundamentales sobre la información que dejamos expuesta y herramientas para su recolección [7].

*   **[Have I Been Pwned](https://haveibeenpwned.com/)**: Rastreo de correos en bases de datos hackeadas [8-10].
*   **[EmailHippo](https://tools.emailhippo.com/)**: Herramienta para verificar la existencia real de un servidor de correo [8, 11, 12].
*   **[This Person Does Not Exist](https://www.thispersondoesnotexist.com/)**: Generación de rostros sintéticos mediante IA para conceptos de ingeniería social [8, 10, 11].
*   **[Fake Name Generator](https://www.fakenamegenerator.com/)**: Creación de identidades sintéticas para perfiles de investigación [8, 10, 11].
*   **[SimpleLogin](https://simplelogin.io/) / Email Aliases**: Gestión de alias para correos (Ej. `omespino+leak@gmail.com`) para protección de identidad y rastreo de fugas [8, 10, 11].

---

## 2. Explotación de Fuentes Públicas y Registros (México) 🇲🇽
Uso de registros de acceso público para localizar información específica [7].

*   **[SEP (Registro Nacional de Profesionistas)](https://www.cedulaprofesional.sep.gob.mx/)**: Verificación de Cédulas Profesionales por nombre completo [2, 8, 11].
*   **[SAT (Servicio de Administración Tributaria)](https://www.sat.gob.mx/)**: 
    *   Generación y validación de RFC mediante CURP [8, 11].
    *   Listas Negras (Art. 69-B) para consulta nacional de empresas fantasma (EFOS/EDOS) [8, 13, 14].
    *   Validación de Facturas CFDI para verificar autenticidad de facturas de compra/venta [13, 15].
*   **[PNT (Plataforma Nacional de Transparencia)](https://www.plataformadetransparencia.org.mx/)**: Buscador maestro de contratos, sueldos y facturas de cualquier nivel de gobierno [13, 14].
*   **[Banxico (Buscador SPEI)](https://www.banxico.org.mx/cep/)**: Validación del titular real de una cuenta bancaria mediante el rastreo de transferencias [13, 14].

---

## 3. Poder Judicial (Investigación Legal) ⚖️
Buscadores públicos para rastrear demandas, amparos y pleitos legales [14].

*   **[SISE (Poder Judicial de la Federación)](https://sise.cjf.gob.mx/sise/)**: Búsqueda de amparos y juicios federales en los 32 estados [13, 14].
*   **[SCJN (Buscador de Sentencias)](https://bj.scjn.gob.mx/)**: Consulta de jurisprudencias y resoluciones de la Suprema Corte [13, 14].
*   **[Boletines Judiciales Estatales (Ej. PJEBC, CDMX)](https://www.pjebc.gob.mx/boletin)**: Portales específicos para pleitos civiles, mercantiles y familiares [13, 15].

---

## 4. Seguridad Patrimonial y Vehicular 🚗🏠
Búsqueda de propiedades, estatus de vehículos y reportes de robo [15].

*   **[REPUVE](http://www2.repuve.gob.mx:8080/ciudadania/)**: Consulta nacional de reporte de robo de vehículos con placa o NIV [2, 13, 15].
*   **[Hacienda BC (Ventanilla Única)](https://tramites.ebajacalifornia.gob.mx/ventanillaunica/tramites/controlvehicular)**: Revisión de adeudo vehicular utilizando el número de placa [2, 13].
*   **[AMIS](https://www.amis.com.mx/)**: Consulta de pólizas de seguro vigentes y reportes de siniestros [13, 15].
*   **[RPP (Registro Público de la Propiedad - BC)](https://rppc.bajacalifornia.gob.mx/)**: Consulta de folios reales, situación legal y estatus de inmuebles mediante claves catastrales o dirección [2, 13, 15].

---

## 5. Análisis Forense, Metadatos y OSINT Físico 🔍
Extracción de datos ocultos para obtener contexto adicional [7].

*   **[ExifTool (Desktop Install)](https://exiftool.org/install.html)**: Extracción profunda de metadatos en imágenes (GPS, fechas, dispositivos, rutas de red) [16-18].
*   **[ExifTools (Web Alternativa)](https://exiftools.com/)**: Interfaz online para leer metadatos de imágenes y documentos [18].
*   **[ArcGIS Wayback Machine](https://livingatlas.arcgis.com/wayback/#mapCenter=-102.39381%2C23.78874%2C20&mode=explore&active=22869)**: Comparativa histórica satelital de mapas y lugares [12, 13].
*   **[KeyMe](https://www.key.me/)**: Riesgos de algoritmos visuales para clonación y decodificación de llaves físicas con solo una fotografía [16, 17].
*   **Conceptos de OSINT Físico**: Información expuesta en gafetes, uniformes, registros de visita de empresas y la recuperación de discos duros de fotocopiadoras que guardan información escaneada históricamente [12, 16, 18].

---

## 6. Correlación, Pivoting y Redes Sociales 🌐
Técnicas para conectar datos dispersos (un correo, un nombre de usuario) y ampliar la superficie de investigación [9, 17].

*   **[TrueCaller Web](https://www.truecaller.com/auth/sign-in?login=phone)**: Identificación de nombres reales asociados a números telefónicos [17-19].
*   **[WhatsMyName.app](https://whatsmyname.app/)**: Búsqueda masiva de un alias de usuario en más de 500 plataformas [17-19].
*   **[X / Twitter Advanced Search](https://x.com/search-advanced)**: 
    *   Filtros por usuario, fechas y lenguaje (`lang:en`) [10, 19, 20].
    *   **Búsqueda por Geocode**: [Ejemplo práctico Coordenadas](https://x.com/search?q=geocode%3A32.62781%2C-115.45446%2C10km&src=typed_query&f=top) [10, 19, 20].
*   **[Mastodon Explore](https://mastodon.social/explore)**: Búsquedas en redes federadas [10, 19].
*   **[Anon Insta Stories](https://insta-stories-viewer.com/)**: Visualización anónima de historias en Instagram [12, 19].
*   **[Tineye](https://tineye.com/) / [Google Lens](https://lens.google/)**: Búsqueda inversa de imágenes para detectar perfiles falsos o fotos robadas [20].
*   **[ScamAdviser](https://www.scamadviser.com/) / WhosID**: Evaluación de reputación de tiendas en línea y perfiles de vendedores [20].

### Casos de Estudio y Extracción Corporativa 🏢
*   **[RocketReach OXXO Profile](https://rocketreach.co/oxxo-profile_b5cff26ff42e0a77)**: Extracción de contactos corporativos, correos y teléfonos de directivos [17-19].
*   **[RocketReach Websec Profile](https://rocketreach.co/websec-profile_b4030d12fc097db9)**: Extracción de información de la empresa [18, 19].
*   **[Prezi Caso Eulises](https://prezi.com/p/xpy7dybtvqdt/objetivo-mensual-de-ventas-junio-2025/)**: Demostración de fugas de datos expuestos en presentaciones públicas (ej. objetivos de ventas) [18, 19].

---

## 7. Repositorios Maestros y Frameworks 📚
Software y frameworks diseñados para automatizar la búsqueda y recolección [9].

*   **[OSINT Framework](https://osintframework.com/)**: Estructura de navegación para organizar tu investigación [12, 19].
*   **[GitHub - OSINT by Aaxash](https://github.com/Aaxash/OSINT?tab=readme-ov-file)**: Biblioteca maestra y repositorio gigante con herramientas actualizadas [18-20].
*   **[Google Guide (Advanced Operators PDF)](https://www.googleguide.com/print/adv_op_ref.pdf)**: Cheat sheet oficial para el dominio de Google Dorks [8, 10, 20].
*   **[VisualPing](https://visualping.io/)**: Herramienta de monitoreo de cambios en sitios web, ideal para defacement o actualizaciones de registros [10, 19, 20].

---

## 8. Recursos Adicionales del Taller 📝
*   **[Página Oficial del Taller - TropiCON 2026](https://tropicon.org/workshops/osint-tactics-what-the-internet-knows-about-you-that-you-didnt-know-about-by-omar-espino/)**
*   **[GitHub - Maigret](https://github.com/soxoj/maigret?tab=readme-ov-file)**: Búsqueda masiva de un mismo alias [17, 19].
*   **[GitHub - Curso OSINT 2022 Academia](https://github.com/aztr4x/CursoOSINT2022_Academia?tab=readme-ov-file)**

---
*Gracias por asistir. Mantén tu higiene digital y reduce tu exposición propia [9].*