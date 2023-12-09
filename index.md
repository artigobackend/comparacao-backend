<link rel="stylesheet" href="{{ 'assets/styles.css' }}">

# Cenários de teste
### 1. [Teste de Pico](#teste-de-pico)
### 2. [Teste de Carga Crescente](#teste-de-carga-crescente)
### 3. [Teste de Resistência](#teste-de-resistência)

# Teste de Pico 

### Sumarização dos dados ([execuções](pages/pico.md))

| Teste de Pico               | Node.js | Django  | .NET   |
|-----------------------------|---------|---------|--------|
| Consumo CPU (%)             | 3,37    | 5,54    | 34,35  |
| Consumo MEMÓRIA (%)         | 0,79    | 0,74    | 18,56  |
| Tempo resposta Total (ms)   | 126,17  | 521,19  | 39,61  |
| DELETE (ms)                 | 123,68  | 269,19  | 57,40  |
| GET (ms)                    | 127,85  | 199,62  | 31,73  |
| POST (ms)                   | 125,70  | 1311,28 | 36,38  |
| PUT (ms)                    | 127,44  | 281,41  | 32,99  |

### Coeficiente de variação (CV) do tempo de resposta dos métodos HTTP entre os Frameworks

| Método | Val. Max. | Média | CV    |
|--------|-----------|-------|-------|
| DELETE | 269,2     | 150,1 | 72,2% |
| GET    | 199,6     | 119,7 | 70,4% |
| POST   | 1311,3    | 491,1 | 144,9%|
| PUT    | 281,4     | 147,3 | 85,1% |
| **Soma Total CV** | | | **372,6%** |

### Coeficiente de variação (CV) do tempo de resposta total dos métodos HTTP entre as execuções

| Coeficiente de Variação (Tempo de resposta total) | Node.js | Django | .NET  |
|--------------------------------------------------|---------|--------|-------|
| **Valor**                                        | 4,20%   | 7,66%  | 0,34% |

# Teste de Carga Crescente

### Sumarização dos dados ([execuções](pages/crescente.md))

| Teste de Carga Crescente    | Node.js | Django  | .NET   |
|-----------------------------|---------|---------|--------|
| Consumo CPU (%)             | 3,32    | 5,5     | 37,74  |
| Consumo MEMÓRIA (%)         | 0,77    | 0,93    | 20,04  |
| Tempo resposta Total (ms)   | 97,15   | 331,31  | 26,74  |
| DELETE (ms)                 | 91,12   | 266,34  | 34,16  |
| GET (ms)                    | 96,35   | 221,20  | 21,20  |
| POST (ms)                   | 99,39   | 545,55  | 28,34  |
| PUT (ms)                    | 101,66  | 286,37  | 23,26  |

### Coeficiente de variação (CV) do tempo de resposta dos métodos HTTP entre os Frameworks

| Método | Val. Max. | Média | CV    |
|--------|-----------|-------|-------|
| DELETE | 266,3     | 130,5 | 92,7% |
| GET    | 221,2     | 112,9 | 89,5% |
| POST   | 545,6    | 224,4 | 124,9% |
| PUT    | 286,4     | 137,1 | 98,5% |
| **Soma Total CV** | | | **405,6%** |

### Coeficiente de variação (CV) do tempo de resposta total dos métodos HTTP entre as execuções

| Coeficiente de Variação (Tempo de resposta total) | Node.js | Django | .NET  |
|--------------------------------------------------|---------|--------|-------|
| **Valor**                                        | 0,61%   | 6,68%  | 1,46% |


# Teste de Resistência

### Sumarização dos dados ([execuções](pages/resistencia.md))

| Teste de Resistência          | Node.js | Django | .NET   |
|-------------------------------|---------|--------|--------|
| Consumo CPU (%)               | 2,85    | 9,22   | 41,11  |
| Consumo MEMÓRIA (%)           | 0,61    | 0,56   | 25,33  |
| Tempo resposta Total (ms)     | 39,13   | 75,59  | 9,74   |
| DELETE (ms)                   | 30,84   | 82,45  | 11,98  |
| GET (ms)                      | 30,64   | 77,47  | 4,67   |
| POST (ms)                     | 46,92   | 33,64  | 12,30  |
| PUT (ms)                      | 48,10   | 108,80 | 9,99   |

### Coeficiente de variação (CV) do tempo de resposta dos métodos HTTP entre os Frameworks

| Método | Val. Max. | Média | CV    |
|--------|-----------|-------|-------|
| DELETE | 82,5      | 41,8  | 87,4% |
| GET    | 77,5      | 37,6  | 98,1% |
| POST   | 46,9      | 31,0  | 56,4% |
| PUT    | 108,8     | 55,6  | 89,6% |
| **Soma Total CV** | | | **331,5%** |

### Coeficiente de variação (CV) do tempo de resposta total dos métodos HTTP entre as execuções

| Coeficiente de Variação (Tempo de resposta total) | Node.js | Django | .NET  |
|--------------------------------------------------|---------|--------|-------|
| **Valor**                                        | 7,49%   | 0,28%  | 9,65% |
