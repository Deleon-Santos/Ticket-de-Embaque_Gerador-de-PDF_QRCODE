# Documentação do Gerenciador de Tickets de Embarque

O **Gerenciador de Tickets de Embarque** é um sistema desenvolvido em Python utilizando a biblioteca PySimpleGUI para interface gráfica, ReportLab para geração de PDFs e qrcode para geração de códigos QR.

## Objetivo

O objetivo do sistema é permitir o cadastro de informações de passageiros para emissão de um ticket de embarque contendo um código QR que pode ser usado para verificar e validar as informações do passageiro.

## Funcionalidades Principais

- **Cadastro de Informações**:
  - O sistema permite o preenchimento de informações como nome completo, número de passaporte, gênero, data de partida, data de retorno e destino.

- **Geração de QR Code**:
  - Com base nas informações inseridas, o sistema gera um código QR contendo os detalhes do passageiro.

- **Geração de PDF**:
  - Um PDF é criado contendo as informações do passageiro e o código QR correspondente.

## Componentes Utilizados

- **PySimpleGUI**:
  - Biblioteca para criação de interfaces gráficas simples e intuitivas.

- **ReportLab**:
  - Biblioteca utilizada para gerar documentos PDF com elementos gráficos e texto.

- **qrcode**:
  - Biblioteca para geração de códigos QR a partir de dados textuais.

## Estrutura do Código

O código está estruturado em Python e utiliza loops de eventos para capturar interações do usuário. As principais funções do sistema são:

- **informacao(valores)**:
  - Recebe os valores inseridos pelo usuário e os formata em uma string contendo as informações do passageiro.

- **gerar_qrcode(data)**:
  - Gera um código QR a partir dos dados fornecidos.

- **criar_pdf(content, qr_filename)**:
  - Cria um arquivo PDF contendo as informações do passageiro e o código QR correspondente.

## Uso

1. Execute o código Python em um ambiente compatível.
2. Preencha os campos solicitados com as informações do passageiro.
3. Clique no botão "RESERVAR" para gerar o ticket de embarque.
4. Um arquivo PDF será gerado e exibido como pop-up informando o nome do arquivo.

## Requisitos

- Python 3.x instalado.
- Bibliotecas PySimpleGUI, ReportLab e qrcode instaladas.
- Desenvolvedor: Deleon Santos
---


