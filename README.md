# 🏎️ Project Tandem — Android ARM64

**Recompilação nativa de Mario Kart: Double Dash!! para dispositivos Android, com renderização acelerada por GPU, controles touchscreen e suporte a dispositivos ARM64.**

O **Project Tandem Android** é um projeto independente de desenvolvimento e engenharia de software que busca executar Mario Kart: Double Dash!! diretamente em dispositivos Android por meio de um motor recompilado para a arquitetura ARM64.

O objetivo é adaptar a execução originalmente destinada ao Nintendo GameCube para o ambiente Android, explorando recompilação nativa, integração gráfica, gerenciamento de memória, processamento de áudio e adaptação dos controles para telas sensíveis ao toque.

O projeto está em desenvolvimento contínuo, com foco em desempenho, compatibilidade e melhorias na experiência de utilização.

## 🎮 Funcionalidades

### 🚀 Execução nativa ARM64

O Project Tandem utiliza código recompilado para a arquitetura ARM64, permitindo executar componentes do jogo diretamente no processador do dispositivo.

A proposta é reduzir a dependência de interpretação contínua das instruções originais, aproveitando os recursos do hardware Android.

### 🎨 Renderização gráfica OpenGL ES

O motor gráfico utiliza OpenGL ES para apresentar os elementos visuais do jogo.

Entre os componentes trabalhados estão:

- Renderização de cenários, personagens e veículos.
- Processamento de texturas e geometria.
- Integração com a GPU do dispositivo.
- Gerenciamento de superfícies e contexto gráfico EGL.
- Ajustes de compatibilidade e correções de renderização.

A implementação continua recebendo melhorias para aumentar a fidelidade visual e a estabilidade.

### 🔊 Sistema de áudio

O projeto possui integração de áudio para reprodução dos sons do jogo, incluindo efeitos sonoros e músicas, com adaptações para o ambiente Android.

### 🕹️ Controles touchscreen

Interface de controles virtuais desenvolvida para dispositivos com tela sensível ao toque.

**Controles disponíveis:**

- Analógico virtual para movimentação.
- Botões A, B, X e Y.
- Botão Z.
- Botões L e R.
- Botão START.
- Controles com transparência para melhorar a visualização da tela.

O objetivo é oferecer uma experiência de controle adequada ao uso em smartphones.

### 💾 Gerenciamento de ISO

O Project Tandem utiliza uma imagem ISO do jogo fornecida pelo próprio usuário.

O sistema de carregamento foi projetado para trabalhar com os mecanismos de acesso a arquivos do Android, incluindo o Storage Access Framework (SAF).

A configuração de armazenamento busca oferecer:

- Seleção da ISO pelo usuário.
- Validação da imagem do jogo.
- Armazenamento privado da referência ao arquivo.
- Persistência da permissão de acesso.
- Carregamento automático nas próximas inicializações, enquanto o arquivo e sua permissão permanecerem válidos.
- Organização das ISOs em uma pasta dedicada ao Project Tandem.

**O projeto não distribui arquivos ISO nem conteúdo comercial do jogo.**

### ⚙️ Configuração e compatibilidade

O aplicativo foi desenvolvido considerando as particularidades do Android moderno.

Entre os recursos de integração estão:

- Gerenciamento de permissões de armazenamento.
- Configurações privadas do aplicativo.
- Inicialização do motor recompilado.
- Integração entre Java, JNI e bibliotecas nativas C/C++.
- Gerenciamento de memória e recursos gráficos.
- Tratamento de falhas e diagnóstico de execução.
- Melhorias de estabilidade e compatibilidade.

## 📱 Requisitos

| Componente | Requisito |
|---|---|
| Plataforma | Android |
| Arquitetura | ARM64 / arm64-v8a |
| Gráficos | GPU compatível com OpenGL ES |
| Armazenamento | Espaço para aplicativo e ISO |
| Jogo | ISO compatível de Mario Kart: Double Dash!! |
| Estado | Desenvolvimento experimental |

O desempenho e a compatibilidade podem variar conforme o dispositivo, a GPU, os drivers e a versão do Android.

## Screenshots

Ainda não há uma captura pública aprovada nesta árvore. As imagens Android encontradas localmente foram rejeitadas porque uma estava sem imagem do jogo e outra incluía dados pessoais da tela de multitarefa. Uma nova captura limpa será adicionada quando um dispositivo Android com o Project Tandem estiver disponível.

## 🛠️ Tecnologias utilizadas

- C e C++
- Java e JNI
- Android NDK
- ARM64
- OpenGL ES
- EGL
- CMake e Ninja
- Recompilação de código nativo
- Storage Access Framework

## 🐧 Versão para Linux

O Project Tandem também possui uma versão desenvolvida para sistemas Linux.

A versão Linux faz parte da evolução técnica do projeto e serve como referência para o desenvolvimento, os testes e a adaptação do motor para outras plataformas.

**Repositório da versão Linux:**

https://github.com/slex2jf/Project-Tandem-Linux

## 🔧 Estado do desenvolvimento

O Project Tandem Android é experimental e continua em evolução.

O trabalho envolve melhorias na renderização, correções de compatibilidade, otimizações de desempenho, estabilidade do motor, integração de áudio e aperfeiçoamento da interface touchscreen.

Nem todas as funcionalidades estão necessariamente completas ou disponíveis em todos os dispositivos.

## 📌 Aviso importante

Este é um projeto independente, desenvolvido para fins de estudo, pesquisa e experimentação técnica.

O Project Tandem não é afiliado, patrocinado ou oficialmente associado à Nintendo.

Mario Kart: Double Dash!!, Nintendo GameCube e demais marcas mencionadas pertencem aos seus respectivos titulares.

Nenhum arquivo comercial do jogo é fornecido com o projeto.

---

**🏁 Project Tandem Android — Levando a recompilação nativa para uma nova plataforma.**
