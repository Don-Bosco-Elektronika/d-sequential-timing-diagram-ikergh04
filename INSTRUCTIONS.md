# 🛠️Zirkuitu Sekuentzialen Kronograma

| **Alumnos** | **Curso** | **Módulo** |
|-------------|-----------|------------|
| 2ME         | 1º        | EEM (Equipos Microprogramables) |

---

## 📌 Ariketa



**Ariketa (EU): (ZENBAKIA IDATZI)**  
| Izena                     | Txip Zenbakia | Sinboloa         | Funtzionamendu Describapena                                                                |
|---------------------------|------------------|------------------|---------------------------------------------------------------------------------|
|D|74100| <img width="118" height="69" alt="Captura de pantalla 2026-01-21 135853" src="https://github.com/user-attachments/assets/3b710569-fc76-4746-94fc-70d4a6636310" />| TTL memoria/flip-flop zirkuitua. Datu digitalak gordetzeko erabiltzen da. |  

| Izena                     | Txip Zenbakia | Sinboloa         | Funtzionamendu Describapena                                                                |
|---------------------------|------------------|------------------|---------------------------------------------------------------------------------|
|D|74175| <img width="83" height="76" alt="Captura de pantalla 2026-01-21 135732" src="https://github.com/user-attachments/assets/249327d0-04a9-4f18-8553-ac6df521ed29" />| 4 D flip-flop dituen erregistroa. CLK bidez kargatu eta RESET dauka. |  

| Izena                     | Txip Zenbakia | Sinboloa         | Funtzionamendu Describapena                                                                |
|---------------------------|------------------|------------------|---------------------------------------------------------------------------------|
| D |74595            | ? | 8 bit desplazamendu-erregistroa latch-ekin. Irteerak gordeta mantentzen ditu.|  

| Izena                     | Txip Zenbakia | Sinboloa         | Funtzionamendu Describapena                                                                |
|---------------------------|------------------|------------------|---------------------------------------------------------------------------------|
| D | 74165             | ? | 8 bit desplazamendu-erregistroa (paralelo → serie). 8 sarrera irakurri eta seriean ateratzen du. |  

| Izena                     | Txip Zenbakia | Sinboloa         | Funtzionamendu Describapena                                                                |
|---------------------------|------------------|------------------|---------------------------------------------------------------------------------|
| D | 74164             | ? | 8 bit desplazamendu-erregistroa (serie → paralelo). Bitak CLK-rekin mugitzen dira. |  



## Tabla de la verdad

| Entrada A | Entrada B | Entrada C | Salida    | Salida |
|-----------|-----------|-----------|-----------|--------|
| 0         | 0         | 0         | ░0░       | ░0░    |
| 0         | 0         | 1         | ░1░       | ░1░    |
| 1         | 1         | 0         | ░1░       | ░1░    |
| 1         | 1         | 1         | ░0░       | ░0░    |

---

## 🔲Simulatzeko Zirkuituak
<img width="487" height="218" alt="Captura de pantalla 2026-01-20 132727" src="https://github.com/user-attachments/assets/c2926a59-8a68-4e63-8c30-b8386bd85979" />
<img width="520" height="332" alt="Captura de pantalla 2026-01-20 205742" src="https://github.com/user-attachments/assets/5b615876-184e-4b65-aa9b-bf1b0dca281d" />
<img width="747" height="353" alt="Captura de pantalla 2026-01-21 141312" src="https://github.com/user-attachments/assets/77814064-bccf-4c95-a9f7-823bc82ae620" />
<img width="518" height="263" alt="Captura de pantalla 2026-01-21 141349" src="https://github.com/user-attachments/assets/89c3c3f9-3e29-4209-97d7-f4896adc4fbc" />




---

## 🔲Kronogramaren Emaitza
<img width="604" height="122" alt="Captura de pantalla 2026-01-20 124252" src="https://github.com/user-attachments/assets/79b4c271-da1a-4623-ac08-f2efbc43ee4f" />
<img width="821" height="282" alt="Captura de pantalla 2026-01-20 114721" src="https://github.com/user-attachments/assets/7d7e67a5-4fc3-40e5-8dd1-a46c310c91ee" />
<img width="821" height="282" alt="Captura de pantalla 2026-01-20 114721" src="https://github.com/user-attachments/assets/7da65642-f422-4a89-b327-767353605929" />
<img width="750" height="180" alt="Captura de pantalla 2026-01-20 120120" src="https://github.com/user-attachments/assets/164b8ee6-3adb-45a5-9d6a-5409e703863f" />
<img width="920" height="190" alt="Captura de pantalla 2026-01-20 120423" src="https://github.com/user-attachments/assets/fa2eaffb-d37d-4703-83bc-85cda41d303f" />






---


## 🔲Kronogramaren Kodea
Ejercicio 2: D asíncrono

{signal: [

  {name: 'D', wave: 'h.lh.lh.lhl.hl..h'},
 
  {},
  
  {name: 'Q', wave: '1.01.01.010.10..1'},
  
  {name: '-Q', wave: '0.10.10.101.01..0'}

]}

Ejercicio 2: D flanco ascendente

{signal: [

  {name: 'clk', wave: 'P.....',period: 3},
 
  {name: 'D', wave: '10101..0.10.101010'},
  
  {},
 
  {name: 'Q', wave: '1..0.1'},
  
  {name: '-Q', wave: '0..1.0'},

]}

Ejercicio 2: D flanco descendente

{signal: [

  {name: 'clk', wave: 'N.....',period: 3},
  
  {name: 'D', wave: '0101..0101.0..1010'},
 
  {},
  
  {name: 'Q', wave: '0.10.1'},
  
  {name: '-Q', wave: '1.01.0'}

]}

Ejercicio 2: D nivel alto

{signal: [

  {name: 'clk', wave: 'p.......', period: 2},
  
  {name: 'D',   wave: '01010101'},
  
  {},
  
  {name: 'Q',   wave: '0.1.0.1.'},
  
  {name: '-Q',  wave: '1.0.1.0.'}

]}

Ejercicio 2: D nivel alto

{signal: [

  {name: 'clk', wave: 'p.......', period: 2},
  
  {name: 'D',   wave: '01010101'},
  
  {},
  
  {name: 'Q',   wave: '0.1.0.1.'},
  
  {name: '-Q',  wave: '1.0.1.0.'}

]}

Ejercicio 2: D nivel bajo

{signal: [

  {name: 'clk', wave: 'n....', period: 4},
  
  {name: 'D',   wave: '0101..0101.01010.1'},
  
  {},
  
  {name: 'Q',   wave: '0...1...0...1...0.'},
  
  {name: '-Q',  wave: '1...0...1...0...1.'}

]}



---


## 📤Igo

➡️ **Instrucciones:**  
- **EU:** Igo hurrengo fitxategiak. Igotako fitxategi guztiek zure izena eduki behar dute.  
  - Sinboloaren argazki bat.  
  - Proteus fitxategia eta zirkuitu bakoitzaren irudia (captura) Proteusen.  
  - Wavedrom bakoitzaren emaitzaren kaptura (grafikoa bakarrik).  
  - **KONTUZ:** Kronogramaren kodea kodea izan behar da, ez irudi bat.



