# ScreenLink

**Compartilhamento de tela em tempo real, direto entre os participantes.**

O ScreenLink é um aplicativo de compartilhamento de tela em salas privadas, desenvolvido para funcionar como complemento ao Discord.

Crie uma sala, compartilhe um código de 5 caracteres com seus amigos e comece a transmitir sua tela. Os participantes podem assistir às transmissões uns dos outros e conversar pelo chat integrado.

Diferentemente das plataformas tradicionais, o vídeo e o áudio são transmitidos diretamente entre os computadores dos participantes, sem passar por um servidor central de vídeo. Assim, você pode continuar usando o Discord para conversar por voz e deixar o ScreenLink responsável apenas pelo compartilhamento de tela.

---

## 📥 Download

**[⬇ Baixar a versão mais recente](LINK_DO_RELEASE)**

### Como instalar

1. Abra o link acima e acesse a seção **Assets** da versão mais recente.
2. Baixe o arquivo `ScreenLink-Setup-X.X.X.exe`.
3. Execute o instalador e siga as instruções.
4. Abra o ScreenLink pelo atalho na área de trabalho ou pelo menu Iniciar.

Não é necessário instalar nenhum outro programa. Após a primeira instalação, o ScreenLink verifica, baixa e instala atualizações automaticamente.

> **Aviso do Windows:** O instalador ainda não possui assinatura digital. Por isso, o Windows pode exibir o aviso "O Windows protegeu seu computador". Clique em **Mais informações** e depois em **Executar assim mesmo** para continuar.

---

## ✨ Principais recursos

### 🏠 Salas compartilhadas

- Salas identificadas por códigos de 5 caracteres.
- Até **6 participantes simultâneos** por sala.
- Qualquer participante pode compartilhar a própria tela.
- Chat de texto integrado, com notificações de entrada e saída.
- Indicador de ping para cada participante e transmissão.
- A sala permanece ativa enquanto houver alguém conectado.
- Se o criador sair, outro participante assume automaticamente a administração da sala.

### 🖥️ Compartilhamento de tela

Qualquer participante pode iniciar uma transmissão com configurações personalizadas:

| Configuração | Opções |
|---|---|
| Fonte | Tela inteira ou aplicativo específico |
| Resolução | 1080p, 720p, 480p, 360p, 240p ou 144p |
| FPS | 24, 30 ou 60 |
| Bitrate | De 1 a 40 Mbps |
| Codec | Automático ou seleção manual |

A transmissão só começa quando você clica em **Iniciar transmissão**.

As configurações de fonte, resolução, FPS e bitrate podem ser alteradas durante a transmissão, sem que os espectadores precisem se reconectar.

### 👀 Assistir às transmissões

- As transmissões disponíveis aparecem na lista de participantes.
- Clique em **Assistir** para visualizar uma transmissão.
- O vídeo só é enviado para quem escolhe assistir, evitando tráfego desnecessário.
- Cada transmissão suporta até 5 espectadores simultâneos.
- É possível assistir a várias transmissões ao mesmo tempo.
- Controles de volume, ping e interrupção da visualização aparecem ao passar o mouse sobre o vídeo.
- Clique duas vezes no vídeo para entrar em tela cheia.

### 🔊 Áudio do sistema

O ScreenLink transmite somente o áudio do sistema. **O microfone nunca é capturado.**

O comportamento depende da fonte selecionada:

- **Tela inteira:** transmite o áudio geral do sistema.
- **Aplicativo específico:** transmite somente o áudio daquele aplicativo, deixando outros programas, como o Discord, de fora.

Isso permite manter a conversa por voz no Discord sem que o áudio da chamada seja incluído na transmissão.

### ⚡ Codec automático e aceleração por hardware

Ao iniciar, o ScreenLink detecta os recursos disponíveis no computador e seleciona automaticamente o codec mais adequado.

São aproveitadas as tecnologias de aceleração por hardware:

- NVIDIA NVENC
- AMD AMF/VCN
- Intel Quick Sync

A ordem de preferência é:

1. AV1
2. H.265 (HEVC)
3. H.264
4. VP9

Caso não exista aceleração por hardware disponível, o programa utiliza H.264 por software.

A seleção também considera a capacidade de decodificação dos computadores que recebem a transmissão, buscando evitar telas pretas e consumo excessivo de processamento.

Na página de ajustes, você pode visualizar os codecs detectados e o tipo de aceleração disponível. Exemplo:

`AV1: hardware | H265: hardware | H264: hardware`

### 🔄 Atualização automática

O ScreenLink verifica automaticamente se existem novas versões disponíveis.

Quando uma atualização é encontrada:

1. O programa baixa a nova versão em segundo plano.
2. Uma notificação aparece no canto da tela.
3. Basta clicar em **Reiniciar e atualizar**.

Caso prefira, a atualização também pode ser aplicada automaticamente ao fechar o programa.

---

## 💻 Requisitos do sistema

- Windows 11; ou Windows 10 versão 2004 ou superior.
- Build 20348 ou mais recente para captura de áudio de aplicativos específicos.
- Conexão com a internet.

Não é necessário criar uma conta, fazer cadastro ou instalar outros programas.

### 📶 Requisitos de upload

Cada espectador recebe um fluxo de vídeo independente. Portanto, quanto mais pessoas assistirem à sua transmissão, maior será o consumo de upload.

Valores aproximados para transmissões a 60 FPS:

| Resolução | Bitrate sugerido | 1 espectador | 5 espectadores |
|---|---:|---:|---:|
| 1080p | 6–8 Mbps | 8 Mbps | 40 Mbps |
| 720p | 3–5 Mbps | 5 Mbps | 25 Mbps |
| 480p ou inferior | 1–2 Mbps | 2 Mbps | 10 Mbps |

Os valores são estimativas. O consumo real depende das configurações utilizadas.

Se sua conexão não suportar a transmissão, reduza o bitrate, a resolução ou o FPS.

---

## 🚀 Como usar

### 1. Criar uma sala

1. Abra o ScreenLink.
2. Digite seu nome.
3. Clique em **Criar nova sala**.
4. Clique em **Copiar código**.
5. Envie o código de 5 caracteres para seus amigos pelo Discord.

### 2. Entrar em uma sala

1. Abra o ScreenLink.
2. Digite seu nome.
3. Informe o código da sala.
4. Clique em **Entrar na sala**.

### 3. Compartilhar sua tela

1. Dentro da sala, clique em **Compartilhar tela**.
2. Escolha a fonte da transmissão.
3. Configure resolução, FPS e bitrate.
4. Mantenha o codec em **Automático** (recomendado).
5. Clique em **Iniciar transmissão**.

Para encerrar, clique em **Parar transmissão**.

### 4. Assistir à tela de alguém

1. Localize o participante que está transmitindo.
2. Clique em **Assistir** ao lado do nome.
3. Passe o mouse sobre o vídeo para acessar os controles de volume, ping e visualização.

---

## 🔒 Privacidade e segurança

O ScreenLink utiliza comunicação P2P (peer-to-peer) através do WebRTC.

- **Conexão direta:** vídeo, áudio e mensagens são enviados diretamente entre os participantes sempre que possível.
- **Criptografia:** a comunicação é protegida pela criptografia do WebRTC.
- **Servidor de sinalização:** o PeerJS é utilizado apenas inicialmente para que os computadores se encontrem e estabeleçam a conexão.
- **Conexão via relé:** quando uma conexão direta não é possível, o programa utiliza um servidor de retransmissão. Nesse caso, o tráfego continua criptografado, mas a qualidade pode ser afetada.
- **Sem captura de microfone:** o aplicativo nunca acessa o microfone.
- **Sem cadastro:** não é necessário fornecer informações pessoais ou criar uma conta.

> **Importante:** qualquer pessoa que conheça o código de uma sala pode tentar entrar. Compartilhe o código apenas com pessoas de confiança e evite publicá-lo em locais públicos.

---

## ⚠️ Limitações conhecidas

- Disponível somente para Windows.
- Não possui comunicação por voz. Utilize o Discord para conversar.
- O chat não mantém histórico. Quem entra depois não visualiza mensagens anteriores, e as mensagens desaparecem quando a sala é encerrada.
- Resolução máxima de 1080p.
- Alguns aplicativos da Microsoft Store, como Calculadora e Filmes e TV, podem não transmitir áudio ao compartilhar somente a janela do aplicativo.
- Jogos executados em tela cheia exclusiva podem apresentar tela preta. Prefira o modo **Janela sem bordas** ou compartilhe a tela inteira.
- Janelas minimizadas não podem ser capturadas.
- A criação e entrada em salas dependem de um serviço público gratuito de sinalização. Caso ele fique indisponível, não será possível estabelecer novas salas.
- Algumas redes, especialmente aquelas com firewalls corporativos ou restrições de conexão P2P, podem impedir a comunicação entre participantes.

---

## 🛠️ Solução de problemas

| Problema | O que fazer |
|---|---|
| Sala não encontrada | Confira o código e verifique se quem criou a sala ainda está com o programa aberto. |
| A sala existe, mas a conexão não foi concluída | A rede ou o firewall pode estar bloqueando a conexão. Tente novamente ou utilize outra rede. |
| Imagem travando ou com baixa qualidade | Reduza o bitrate, a resolução ou o FPS. |
| Transmissão sem som | Verifique se existe áudio sendo reproduzido e se o dispositivo de saída padrão do Windows está configurado corretamente. |
| Codec automático não detectou o hardware | Abra a página de ajustes e clique em **Detectar hardware** novamente. |
| Tela preta ao compartilhar um jogo | Utilize o modo Janela sem bordas ou compartilhe a tela inteira. |

---

## 🧰 Tecnologias utilizadas

- **Electron:** estrutura do aplicativo desktop.
- **WebRTC:** comunicação em tempo real entre participantes.
- **PeerJS:** sinalização e estabelecimento das conexões P2P.
- **WASAPI:** captura de áudio do sistema operacional Windows.
- **Codecs de vídeo:** AV1, H.265, H.264 e VP9, com suporte à aceleração por hardware quando disponível.

---

## 🎯 Objetivo do projeto

O ScreenLink foi criado para oferecer uma alternativa simples e eficiente ao compartilhamento de tela tradicional em chamadas do Discord.

A proposta é separar a comunicação por voz da transmissão de vídeo, permitindo que cada ferramenta faça aquilo para o qual foi projetada.

**Converse pelo Discord. Compartilhe pelo ScreenLink.**
