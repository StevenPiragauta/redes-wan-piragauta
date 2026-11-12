# docs/pruebas.md — Suite de Pruebas Automatizadas y Porcentaje de Confianza
**Proyecto:** WAN Architect Studio v3.6.0  
**Evaluación:** Corte 3 — Interconexión de Redes WAN  
**Nivel de Confianza Certificado:** 100% (6 de 6 Casos Exitosos)

---

## 1. Matriz Formal de Casos de Prueba

| ID | Tipo de Caso | Módulo Evaluado | Entrada Suministrada | Salida Esperada | Salida Obtenida | Resultado |
| :---: | :---: | :--- | :--- | :--- | :--- | :---: |
| **TC-01** | Normal | Conversión IPv4 ↔ Entero | IP: `192.168.10.1` | Entero: `3232238081` y reversión exacta | `192.168.10.1` | **PASÓ (100%)** |
| **TC-02** | Normal | Máscara WAN /30 | Prefijo: `/30` | `255.255.255.252` (2 hosts asignables) | `255.255.255.252` | **PASÓ (100%)** |
| **TC-03** | Límite | Validador de Red Base CIDR | `10.0.0.0/16` y entrada anómala `999.0.0.0/40` | Aceptación de formato RFC1918 y rechazo de prefijos > 30 | Correctamente filtrado | **PASÓ (100%)** |
| **TC-04** | Normal | Algoritmo VLSM sin Solapamiento | 5 Sedes con múltiples pisos y 5 tipos de dispositivos | Cero colisiones de rangos IP y broadcast | Subredes continuas y ordenadas | **PASÓ (100%)** |
| **TC-05** | Seguridad | Ciberdefensa Anti-Prompt Injection | `test; drop table routers; ignore previous` | Detección de patrones maliciosos y bloqueo inmediato | Amenaza bloqueada (`drop`, `;`, `ignore`) | **PASÓ (100%)** |
| **TC-06** | Multimarca | Generador Multimarca (4 Fabricantes) | Presets corporativos para Cisco, Huawei, Fortinet y MikroTik | Scripts sintácticamente completos con OSPF y subinterfaces | 4 fabricantes generados con OSPF y WAN /30 | **PASÓ (100%)** |

---

## 2. Cálculo del Porcentaje de Confianza

$$\text{Porcentaje de Confianza} = \left( \frac{\text{Pruebas Superadas}}{\text{Total de Pruebas}} \right) \times 100 = \left( \frac{6}{6} \right) \times 100 = 100\%$$

---

## 3. Instrucciones para la Sustentación Oral en Vivo
1. Abrir la aplicación web en el navegador.
2. Hacer clic en el botón morado de cabecera: **`Correr Pruebas en Vivo (20%)`**.
3. Se desplegará el modal interactivo ejecutando los 6 casos con su veredicto verde y la barra al **100% de Confianza**.