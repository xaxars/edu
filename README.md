# 🚣 Analitzador de Palades

Aplicació web per a l'anàlisi biomecànic del rem mitjançant l'extracció de fotogrames clau d'un vídeo lateral.

![Versió](https://img.shields.io/badge/versió-1.0-blue)
![Llicència](https://img.shields.io/badge/llicència-MIT-green)
![Plataforma](https://img.shields.io/badge/plataforma-Web%20%7C%20iPad%20%7C%20Mòbil-orange)

## 📋 Descripció

Aquesta eina permet analitzar la tècnica de rem a partir d'un vídeo gravat des del lateral. Extreu automàticament fotogrames clau de les fases de passada i recuperació, calculant temps i ràtios importants per a l'anàlisi biomecànic.

## ✨ Funcionalitats

- **Càrrega de vídeo**: Des de la galeria o gravació directa (iPad/mòbil)
- **Navegació precisa**: Fotograma a fotograma amb controls tàctils optimitzats
- **Marcadors temporals**:
  - 🔴 Catch (Atac): Inici de la passada
  - 🟢 Sortida: Fi de la passada / Inici recuperació
  - 🔵 Fi Recuperació: Opcional, per a mesures precises
- **Extracció automàtica**: 10 fotogrames (5 passada + 5 recuperació)
- **Estadístiques**: Temps de passada, recuperació, ràtio i cicle total
- **Exportació**: ZIP amb totes les imatges + galeria per iPad

## 🎯 Ús

1. Carrega un vídeo lateral del rem
2. Navega fins al **catch** (quan el capçal mòbil canvia de sentit per iniciar la passada)
3. Marca amb el botó vermell 🔴
4. Navega fins a la **sortida** (quan el capçal canvia de sentit iniciant la recuperació)
5. Marca amb el botó verd 🟢
6. (Opcional) Marca el **fi de recuperació** amb el botó blau 🔵
7. Genera els fotogrames!

## ⌨️ Dreceres de Teclat

| Tecla | Acció |
|-------|-------|
| `Espai` | Reproduir/Pausar |
| `←` | -1 fotograma |
| `→` | +1 fotograma |
| `Shift + ←` | -10 fotogrames |
| `Shift + →` | +10 fotogrames |
| `C` | Marcar Catch |
| `F` | Marcar Sortida (Finish) |
| `R` | Marcar Fi Recuperació |

## 📱 Compatibilitat iPad/iOS

L'aplicació està optimitzada per a dispositius Apple:

- Botons de mida tàctil (44px mínim)
- Reproducció de vídeo inline (sense pantalla completa forçada)
- Galeria d'imatges amb suport per "mantenir premut" per guardar
- Exportació ZIP compatible amb Safari
- Suport per gestos swipe a la galeria

## 🔧 Tecnologies

- HTML5 / CSS3 / JavaScript vanilla
- Canvas API per a captura de fotogrames
- [JSZip](https://stuk.github.io/jszip/) per a generació de ZIP
- Disseny responsiu amb CSS Grid/Flexbox

## 📊 Sortides

### Fotogrames Generats

**Fase de Passada (Drive):**
1. CATCH (Atac)
2. Passada 25%
3. Passada 50%
4. Passada 75%
5. SORTIDA (Fi)

**Fase de Recuperació:**
1. Inici Recuperació
2. Recuperació 25%
3. Recuperació 50%
4. Recuperació 75%
5. Fi Recuperació

### Estadístiques

- Temps de passada (ms)
- Temps de recuperació (ms)
- Ràtio Recuperació/Passada
- Durada del cicle complet

## 🚀 Instal·lació

No cal instal·lació! Simplement:

1. Descarrega o clona el repositori
2. Obre `index.html` al navegador

O accedeix directament via GitHub Pages (si està habilitat).

```bash
git clone https://github.com/[usuari]/analitzador-palades.git
cd analitzador-palades
# Obre index.html al navegador
```

## 📁 Estructura

```
analitzador-palades/
├── index.html      # Aplicació completa (single file)
├── README.md       # Aquest fitxer
└── LICENSE         # Llicència MIT
```

## 🤝 Contribucions

Les contribucions són benvingudes! Si tens suggeriments o trobes errors:

1. Obre un Issue
2. Fes un Fork del repositori
3. Crea una branca (`git checkout -b feature/millora`)
4. Commit els canvis (`git commit -m 'Afegeix millora'`)
5. Push a la branca (`git push origin feature/millora`)
6. Obre un Pull Request

## 📄 Llicència

Aquest projecte està sota la llicència MIT. Consulta el fitxer [LICENSE](LICENSE) per a més detalls.

## 👤 Autor

Desenvolupat per a l'anàlisi tècnic del rem.

---

*Fet amb ❤️ per a la comunitat del rem*
