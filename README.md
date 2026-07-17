K+N Operation Dashboard

Painel de operação (Daily Operation Overview) desenvolvido para a Kuehne+Nagel, com visual inspirado nos dashboards de centros de distribuição de grandes operadores logísticos (Amazon, DHL, Mercado Livre).

Feito para ser exibido em TVs de sala de operação, atualizado em tempo real e editado por qualquer pessoa da equipe através de um painel administrativo, sem necessidade de mexer em código.

Criado por: Anderson Chiesa

✨ Visão geral

O projeto é um único arquivo HTML autossuficiente (kn-operation-dashboard.html), sem backend, sem build, sem dependência de banco de dados. Basta abrir no navegador ou publicar em qualquer serviço de hospedagem estática.

O que foi construído

Identidade visual da Kuehne+Nagel: paleta em tons de azul institucional, branco e cinza claro, com cards em efeito glassmorphism, tipografia Space Grotesk + Inter + JetBrains Mono e logo oficial embutida no cabeçalho.
Cabeçalho com logo, nome da empresa, assinatura "Inspire. Empower. Deliver", título "Daily Operation Overview", relógio em tempo real e data atual por extenso.
4 cards de valores (Segurança em 1º Lugar, Time Forte, Excelência em cada Etapa, Foco em Resultados), cada um com ícone próprio e microanimação ao passar o mouse.
Faixa de Total Geral de HC da operação, somando automaticamente todos os ciclos e turnos.
3 blocos de ciclo — AM0, PM1 e SD — cada um com:

Cor de borda própria (clara → escura, representando o horário do dia)
Lado A e Lado B, com Coordenador, Liderança e HC
Total de HC do ciclo, calculado automaticamente (Lado A + Lado B) com contador animado
Destaque visual automático ("Ciclo Atual") no ciclo correspondente ao horário do relógio


Painel administrativo oculto (botão "⚙ Editar Informações"), com formulário lateral para editar data, coordenadores, lideranças e HC de todos os ciclos. Ao salvar, o dashboard é atualizado instantaneamente, sem recarregar a página.
Persistência de dados: as informações são salvas automaticamente e ficam disponíveis para qualquer pessoa que abra o dashboard — não é necessário reenviar arquivo nem reeditar código a cada turno.
Modo escuro / modo claro com botão de alternância.
Impressão / exportação em PDF (via impressão do navegador), com layout adaptado (esconde botões e painel administrativo).
Totalmente responsivo: layout pensado para TV Full HD, mas também funciona em notebook, tablet e celular.
Ícones em SVG nativo (sem dependência de bibliotecas externas de ícones), garantindo que o visual sempre carregue corretamente.


🛠️ Tecnologias utilizadas

HTML5, CSS3 e JavaScript puro (vanilla) — nenhum framework
Google Fonts (Space Grotesk, Inter, JetBrains Mono)
Ícones SVG inline, desenhados sob medida
API de armazenamento key-value para persistência dos dados (sem necessidade de banco de dados)
