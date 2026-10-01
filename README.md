INFORME DE LABORATORIO — CORTE 2

DISEÑO, AUTOMATIZACIÓN DE REDES WAN CORPORATIVAS Y CIBERDEFENSA APLICADA CONTRA IA

Asignatura: Interconexión de Redes WAN

Docente: John Harold Pérez Calderón
Estudiante: Oscar Steven Piragauta
Programa Académico: Ingeniería de Telecomunicaciones
Enlace al Repositorio Público: https://github.com/StevenPiragauta/redes-wan-piragauta
Versión de la Herramienta: v3.6.0 (WAN Architect Studio)

1. Descripción del ProyectoWAN Architect Studio v3.6.0 es una solución web cliente (SPA) que permite a directores de TI e ingenieros dimensionar planes de direccionamiento IPv4 (VLSM) sin solapamiento, modelar topologías jerárquicas con enlaces WAN /30 y generar scripts multimarca (Cisco IOS, Huawei VRP, Fortinet, MikroTik) integrando ciberdefensa contra inyección de prompts de IA.

2. Estructura del Repositorioredes-wan-piragauta/
├── .gitignore
├── README.md
├── index.html
└── docs/
    ├── informe-corte2.pdf
    ├── politicas-ia.md
    └── capturas/
        ├── 01-subnetting.png
        ├── 02-topologia.png
        ├── 03-config-cisco.png
        ├── 04-config-huawei.png
        ├── 05-github-commits.png
        └── 08-ciberdefensa.png

3. Tabla de Evidencias 

Criterio			Archivo / Evidencia			Descripción							Estado
Subnetting Funcional (20%)	docs/capturas/01-subnetting.png		Tabla VLSM calculada sin colisiones y exportación a Excel.	Cumplido
Carga de Topología (15%)	docs/capturas/02-topologia.png		Esquema jerárquico de sedes WAN y switches de distribución.	Cumplido
Config Cisco (12.5%)		docs/capturas/03-config-cisco.png	Script Cisco IOS con subinterfaces 802.1Q y OSPF.		Cumplido
Config Huawei (12.5%)		docs/capturas/04-config-huawei.png	Script Huawei VRP con terminación dot1Q y proceso OSPF.		Cumplido
Historial GitHub (20%)		docs/capturas/05-github-commits.png	Mínimo 5 commits progresivos y rama de desarrollo.		Cumplido
Ciberdefensa Aplicada (10%)	docs/capturas/08-ciberdefensa.png	Sanitización anti-prompt injection y .gitignore.		mCumplido
