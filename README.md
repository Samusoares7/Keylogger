# Keylogger
Este projeto demonstra, de forma educacional e controlada, o funcionamento básico de um keylogger utilizando Python.


# 🔐 Keylogger Simulado em Python (Ambiente Controlado)

## 📌 Descrição

O script captura entradas do teclado e registra em um arquivo local (`log.txt`), simulando como malwares desse tipo operam na coleta de dados.

> ⚠️ Este projeto foi desenvolvido exclusivamente para fins de estudo em cibersegurança.

---

## 🎯 Objetivo

* Entender como keyloggers capturam entradas do usuário
* Observar como dados podem ser armazenados localmente
* Estudar formas de detecção e prevenção desse tipo de ameaça

---

## 🛠️ Tecnologias utilizadas

* Python 3
* Biblioteca `pynput`

Instalação da dependência:

```bash
pip install pynput
```

---

## ⚙️ Funcionamento

O script utiliza um listener do teclado para capturar cada tecla pressionada.

### Comportamento:

* Letras e números → registrados normalmente
* Espaço → `" "`
* Enter → quebra de linha
* Tab → `\t`
* Backspace → substituído por espaço
* ESC → `[ESC]`
* Teclas especiais (Shift, Ctrl, Alt, etc.) → ignoradas

Todas as entradas são salvas no arquivo:

```
log.txt
```

---

## 📂 Estrutura

```
keylogger/
├── keylogger.py
└── log.txt
```

---

## 🧠 Conceito por trás

Keyloggers são programas que monitoram e registram tudo o que um usuário digita. Em cenários reais, podem ser usados para:

* Roubo de senhas
* Captura de dados sensíveis
* Espionagem

Este projeto simula esse comportamento de forma **limitada e transparente**.

---

## 🛡️ Como se proteger

Algumas boas práticas contra keyloggers:

* Utilizar antivírus atualizado
* Evitar downloads de fontes desconhecidas
* Monitorar processos suspeitos no sistema
* Utilizar autenticação em dois fatores (2FA)
* Preferir teclados virtuais em ambientes sensíveis

---

## ⚠️ Aviso Legal

Este código não deve ser utilizado para fins maliciosos.

O uso é estritamente educacional, com foco em aprendizado de segurança da informação e análise de ameaças.

---

## 🚀 Possíveis melhorias

* Criptografia do arquivo de log
* Simulação de envio dos dados (ambiente controlado)
* Interface para visualização dos logs
* Execução em sandbox para análise segura

---

## 📎 Conclusão

Este projeto ajuda a entender, na prática, como ataques simples podem capturar informações do usuário e reforça a importância de boas práticas de segurança.

---

