# GUÍA DE PÁGINAS A CREAR — FísicaConvert
# Copiá la plantilla metros-a-centimetros.html y modificá estos valores por página

## ESTRUCTURA DE CADA PÁGINA
Cada archivo necesita cambiar:
1. <title> — "Convertir X a Y — Calculadora Online | FísicaConvert"
2. <meta name="description"> — descripción única con la fórmula
3. <link rel="canonical"> — URL exacta de la página
4. <h1> — "Convertir X a Y"
5. Labels del conversor ("Metros (m)" → tu unidad origen, "Centímetros (cm)" → destino)
6. Factor en la función JS: `const resultado = valor * FACTOR;`
7. Textos explicativos, tabla de referencia, FAQ

---

## PÁGINAS PRIORITARIAS — Hacelas primero (más buscadas)

### TEMPERATURA (las más buscadas en física)
| Archivo | Factor JS | Fórmula |
|---|---|---|
| celsius-a-kelvin.html | `resultado = celsius + 273.15` | K = °C + 273,15 |
| celsius-a-fahrenheit.html | `resultado = (celsius * 9/5) + 32` | °F = (°C × 9/5) + 32 |
| fahrenheit-a-celsius.html | `resultado = (f - 32) * 5/9` | °C = (°F − 32) × 5/9 |
| kelvin-a-celsius.html | `resultado = kelvin - 273.15` | °C = K − 273,15 |

### VELOCIDAD (muy buscada en cinemática)
| Archivo | Factor JS | Factor numérico |
|---|---|---|
| kmh-a-ms.html | `resultado = kmh / 3.6` | ÷ 3,6 |
| ms-a-kmh.html | `resultado = ms * 3.6` | × 3,6 |
| kmh-a-mph.html | `resultado = kmh * 0.621371` | × 0,621371 |
| mph-a-kmh.html | `resultado = mph * 1.60934` | × 1,60934 |

### ENERGÍA (muy buscada en termodinámica)
| Archivo | Factor JS | Factor numérico |
|---|---|---|
| joules-a-calorias.html | `resultado = joules / 4.184` | ÷ 4,184 |
| calorias-a-joules.html | `resultado = cal * 4.184` | × 4,184 |
| joules-a-kwh.html | `resultado = joules / 3600000` | ÷ 3.600.000 |
| joules-a-electronvoltios.html | `resultado = joules * 6.242e18` | × 6,242×10¹⁸ |

### FUERZA (indispensable en dinámica)
| Archivo | Factor JS | Factor numérico |
|---|---|---|
| newton-a-kilogramo-fuerza.html | `resultado = newton / 9.80665` | ÷ 9,80665 |
| kilogramo-fuerza-a-newton.html | `resultado = kgf * 9.80665` | × 9,80665 |
| newton-a-libra-fuerza.html | `resultado = newton * 0.224809` | × 0,224809 |
| dina-a-newton.html | `resultado = dina / 100000` | ÷ 100.000 |

### PRESIÓN (muy buscada en fluidos y termodinámica)
| Archivo | Factor JS | Factor numérico |
|---|---|---|
| pascal-a-atm.html | `resultado = pascal / 101325` | ÷ 101.325 |
| pascal-a-bar.html | `resultado = pascal / 100000` | ÷ 100.000 |
| pascal-a-mmhg.html | `resultado = pascal / 133.322` | ÷ 133,322 |
| atm-a-pascal.html | `resultado = atm * 101325` | × 101.325 |
| bar-a-pascal.html | `resultado = bar * 100000` | × 100.000 |
| psi-a-pascal.html | `resultado = psi * 6894.76` | × 6.894,76 |

### LONGITUD (muchas búsquedas cotidianas)
| Archivo | Factor JS | Factor numérico |
|---|---|---|
| metros-a-pies.html | `resultado = metros * 3.28084` | × 3,28084 |
| metros-a-pulgadas.html | `resultado = metros * 39.3701` | × 39,3701 |
| metros-a-milimetros.html | `resultado = metros * 1000` | × 1.000 |
| kilometros-a-millas.html | `resultado = km * 0.621371` | × 0,621371 |
| pies-a-metros.html | `resultado = pies / 3.28084` | ÷ 3,28084 |
| pulgadas-a-centimetros.html | `resultado = pulgadas * 2.54` | × 2,54 |
| millas-a-kilometros.html | `resultado = millas * 1.60934` | × 1,60934 |

### MASA
| Archivo | Factor JS | Factor numérico |
|---|---|---|
| kilogramos-a-gramos.html | `resultado = kg * 1000` | × 1.000 |
| kilogramos-a-libras.html | `resultado = kg * 2.20462` | × 2,20462 |
| libras-a-kilogramos.html | `resultado = libras / 2.20462` | ÷ 2,20462 |
| gramos-a-miligramos.html | `resultado = gramos * 1000` | × 1.000 |
| toneladas-a-kilogramos.html | `resultado = ton * 1000` | × 1.000 |

### ÁNGULO (muy buscado en física y trigonometría)
| Archivo | Factor JS | Factor numérico |
|---|---|---|
| grados-a-radianes.html | `resultado = grados * Math.PI / 180` | × π/180 |
| radianes-a-grados.html | `resultado = rad * 180 / Math.PI` | × 180/π |

### CAMPO MAGNÉTICO (diferenciador único)
| Archivo | Factor JS | Factor numérico |
|---|---|---|
| tesla-a-gauss.html | `resultado = tesla * 10000` | × 10.000 |
| gauss-a-tesla.html | `resultado = gauss / 10000` | ÷ 10.000 |

---

## CHECKLIST POR PÁGINA
- [ ] Título H1 con "Convertir X a Y"
- [ ] Meta description con fórmula mencionada
- [ ] Link canonical correcto
- [ ] Schema HowTo con 3 pasos
- [ ] Schema FAQPage con 3-4 preguntas
- [ ] Tabla de referencia con 8-10 filas
- [ ] 3-4 ejemplos prácticos cotidianos
- [ ] Links a conversiones relacionadas
- [ ] Slot de AdSense preparado

---

## ORDEN DE PRIORIDAD SUGERIDO
1. celsius-a-kelvin (la más buscada en física)
2. celsius-a-fahrenheit
3. joules-a-calorias
4. newton-a-kilogramo-fuerza
5. pascal-a-atm
6. kmh-a-ms
7. grados-a-radianes
8. kilogramos-a-libras
9. tesla-a-gauss (diferenciador)
10. joules-a-electronvoltios (diferenciador)
