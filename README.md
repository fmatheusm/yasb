# Configuração do YASB

Esta pasta contém a configuração da barra do [YASB](https://github.com/amnweb/yasb) no Windows. A configuração principal está em `config.yaml`; aparência e cores ficam em arquivos CSS separados.

## Visão geral

A barra principal está habilitada e aparece no topo da tela principal, centralizada, com 28 px de altura. Ela usa animações, efeito de desfoque e o modo de barra de aplicativos do Windows.

Os widgets são organizados em três áreas:

| Área | Widgets, da esquerda para a direita |
| --- | --- |
| Esquerda | Início, inicializador de aplicativos, áreas de trabalho virtuais e janela ativa |
| Centro | Clima, relógio e atualizações do WinGet |
| Direita | Visualizador de áudio, mídia, bandeja do sistema, monitor do sistema, microfone, volume, notificações e menu de energia |

## Widgets

| Widget | O que exibe ou faz |
| --- | --- |
| **Início** | Abre um menu com atalhos para a pasta pessoal, Downloads, Documentos e Imagens, além dos menus de sistema e energia. |
| **Inicializador de aplicativos** | Pesquisa aplicativos instalados, exibe ícones e resultados recentes. Pode ser aberto com `Alt` + `Espaço`. |
| **Áreas de trabalho** | Mostra os desktops virtuais do Windows; a rolagem permite alternar entre eles. |
| **Janela ativa** | Mostra o título da janela em foco, com ícone, limitado a 32 caracteres. |
| **Clima** | Exibe a temperatura e oferece um cartão com previsão de até sete dias e previsão horária. Usa unidades métricas e ícones para as condições climáticas. |
| **Relógio** | Exibe dia, data e hora; o rótulo alternativo mostra a data completa em português do Brasil. O calendário usa feriados do Brasil. |
| **Atualizações** | Consulta atualizações do WinGet a cada 240 segundos. A verificação de atualizações do Windows e do Scoop está desativada. |
| **Visualizador de áudio** | Mostra barras de frequência em estéreo convertido para mono; fica oculto quando não há áudio após o período de inatividade configurado. |
| **Mídia** | Exibe título e artista, miniatura, barra de progresso e controles de reprodução. |
| **Bandeja do sistema** | Agrupa os ícones da área de notificação em um pop-up. Bateria, volume e ícones não fixados não são exibidos diretamente. |
| **Monitor do sistema** | Agrupa CPU, memória e GPU. Os widgets individuais exibem métricas e oferecem menus com gráficos. |
| **Microfone** | Indica o estado do microfone e permite abrir o menu ou alternar o mudo. |
| **Volume** | Mostra o nível de áudio e permite abrir o mixer ou alternar o mudo. O mixer pode exibir os volumes dos aplicativos. |
| **Notificações** | Abre a central de notificações; o widget é ocultado quando não há notificações. |
| **Menu de energia** | Abre ações de bloquear, sair, suspender, hibernar, reiniciar e desligar. |

## Aparência e arquivos

- [`config.yaml`](./config.yaml) define a barra, a posição dos widgets, opções e ações de mouse/teclado.
- [`styles.css`](./styles.css) define a aparência da barra e dos widgets. O tema usa fundo preto, texto claro e destaque azul-claro, além de estilos para menus, pop-ups e tooltips.
- [`yasb_colors.css`](./yasb_colors.css) contém variáveis de cores geradas pelo YASB; o próprio arquivo recomenda importá-lo em `styles.css`.

O monitoramento de alterações de configuração e de estilos está habilitado em `config.yaml`, assim como a verificação de atualizações do YASB. Para personalizar a barra, edite as opções do widget correspondente em `config.yaml`; para mudar cores, fontes ou espaçamento, ajuste `styles.css`.
