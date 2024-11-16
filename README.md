# Projeto de Automação de Testes para Dispositivos Móveis com Robot e Appium

Este projeto é destinado à automação de testes para aplicativos móveis para gerenciamento de tarefas usando Robot Framework e Appium, garantindo uma abordagem eficiente e escalável para validar a funcionalidade de aplicativos Android


## Tabela de Conteúdos
1. Estrutura do Projeto
2. Pré-requisitos
3. Configuração do Ambiente
4. Execução dos Testes

## Estrutura do Projeto
📂 MARKX-ROBOT
├── 📁 apps              # Arquivos do aplicativo em teste
├── 📁 logs              # Logs gerados durante a execução dos testes
├── 📁 node_modules      # Dependências gerenciadas pelo Node.js
├── 📁 resources         # Recursos do Robot Framework
├── 📁 tests             # Casos de teste em Robot Framework


## Descrição das Pastas
apps: Contém os arquivos ou links para o APK ou IPA do aplicativo sob teste.
logs: Repositório dos logs e relatórios gerados após a execução dos testes.
node_modules: Pasta gerada automaticamente pelo gerenciador de pacotes Node.js.
resources: Scripts reutilizáveis, variáveis ou funções específicas para suporte aos testes.
tests: Casos de teste em formato .robot.

### Pré-requisitos
Certifique-se de ter os seguintes requisitos instalados:

## Softwares Necessários
Java: 22.0.2
Android Studio: Koala 2024.1.1 Patch 1
Appium: 2.1.3

## Configurações Adicionais
Emulador Android: Pixel 3a (API 35).
Node.js: Para gerenciar as dependências do Appium.
Robot Framework: Incluído no arquivo requirements.txt.

### Configuração do Ambiente

## 1. Instalar Dependências
Execute o seguinte comando para instalar as bibliotecas necessárias:
pip install -r requirements.txt

## 2. Configurar o Appium
1. Instale o Appium globalmente:
npm install -g appium

2. Verifique se o Appium está funcionando:
appium --version

## 3. Configurar o Emulador
1. Abra o Android Studio.
2. Configure um emulador Pixel 3a com API 35.
3. Certifique-se de que o emulador está ativo antes de iniciar os testes.

### Execução dos Testes
npx appium
robot -d logs tests/

Os resultados detalhados estarão disponíveis na pasta logs, incluindo relatórios no formato HTML.# markx-appium-robot
