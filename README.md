# Encriptador e Desencriptador de Arquivos

Este projeto demonstra como encriptar e desencriptar arquivos usando a biblioteca `pyaes` em Python. Ele contém dois scripts separados para realizar as operações de criptografia e descriptografia em um arquivo de texto.

## Arquivos e Funções

### 1. Script de Criptografia (`encrypt.py`)
Este script realiza as seguintes etapas:
1. Abre um arquivo chamado `arquivo.txt` e lê seu conteúdo.
2. Remove o arquivo original para evitar duplicação.
3. Encripta os dados usando o algoritmo AES no modo CTR, com uma chave pré-definida.
4. Salva os dados encriptados em um novo arquivo chamado `arquivo.txt.ransomware`.

#### Resultado da criptografia:
Após executar este script, o arquivo original (`arquivo.txt`) será substituído pelo arquivo encriptado (`arquivo.txt.ransomware`).  
O conteúdo do arquivo encriptado será ilegível, semelhante ao exemplo abaixo:
�����S�tl��xG�ba�*�j��0���

---

### 2. Script de Descriptografia (`decrypt.py`)
Este script reverte o processo de criptografia:
1. Abre o arquivo encriptado `arquivo.txt.ransomware` e lê seus dados.
2. Remove o arquivo encriptado para evitar duplicação.
3. Desencripta os dados usando o algoritmo AES no modo CTR, com a mesma chave usada na criptografia.
4. Salva os dados descriptografados em um novo arquivo chamado `arquivo.txt`.

#### Resultado da descriptografia:
Após executar este script, o arquivo encriptado (`arquivo.txt.ransomware`) será substituído pelo arquivo original recuperado (`arquivo.txt`).  
O conteúdo do arquivo recuperado será o texto original, como no exemplo:
Você está lendo este arquivo

---

## Como Usar

### Pré-requisitos
- Python instalado em seu sistema.
- Biblioteca `pyaes` instalada. Para instalar, use no terminal:
  pip install pyaes

Criptografar
Salve o script de criptografia como encrypter.py e execute-o no terminal:

python encrypt.py

---

Descriptografar
Salve o script de descriptografia como decrypter.py e execute-o no terminal:

python decrypt.py
