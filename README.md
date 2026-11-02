ScreenLink
Compartilhamento de tela em sala, direto entre os participantes, feito para ser um complemento ao Discord.
![Versão](https://img.shields.io/github/v/release/ThomasArielxl/screenlink-releases?label=vers%C3%A3o&color=5ec2a8)
![Plataforma](https://img.shields.io/badge/plataforma-Windows%2010%2F11-blue)
O ScreenLink cria uma sala com um código de 5 caracteres. Quem entra pode transmitir a própria tela, assistir às transmissões dos outros e conversar por texto. O vídeo e o áudio vão direto de um PC para o outro, sem passar por um servidor de vídeo. Você mantém a conversa de voz no Discord e usa o ScreenLink só para a imagem, com mais qualidade e controle.
---
Baixar
⬇ Baixar a versão mais recente
Abra o link acima e, na seção Assets, clique em `ScreenLink-Setup-X.X.X.exe`.
Execute o arquivo baixado e siga o instalador.
Abra o ScreenLink pelo atalho da área de trabalho ou do menu Iniciar.
Não é preciso instalar mais nada. Depois da primeira instalação, o programa se atualiza sozinho.
> **Aviso do Windows:** o instalador ainda não tem assinatura digital, então o Windows pode mostrar "O Windows protegeu seu computador". Clique em **Mais informações** e depois em **Executar assim mesmo**.
---
Principais recursos
Sala
Código de 5 caracteres. Um participante cria a sala e envia o código pelo Discord. Os outros digitam o código e entram.
Até 6 pessoas por sala.
Chat de texto dentro da sala, com aviso de quem entra e sai.
Ping de cada participante na lista e em cada transmissão, para você saber como está a conexão.
A sala continua enquanto houver alguém dentro. Se quem criou sair, outro participante assume.
Compartilhar tela
Qualquer pessoa da sala pode transmitir. Ao clicar em Compartilhar tela, abre uma página de ajustes com:
Ajuste	Opções
Fonte	Tela inteira ou um aplicativo específico aberto
Resolução	Até 1080p: 1080p, 720p, 480p, 360p, 240p e 144p
FPS	24, 30 ou 60 FPS
Bitrate	De 1 a 40 Mbps, ajustável ao vivo
Codec	Automático (recomendado) ou escolha manual
A transmissão só começa quando você clica em Iniciar transmissão. Você pode mudar fonte, resolução, FPS e bitrate durante a transmissão, sem os espectadores precisarem reconectar.
Assistir
Quem está transmitindo aparece na lista de participantes com o botão Assistir.
O vídeo só é enviado para quem clica em Assistir, o que poupa a internet de quem transmite.
Cada transmissão aceita até 5 espectadores ao mesmo tempo.
Dá para assistir a várias transmissões ao mesmo tempo.
Controles de volume, ping e Parar de assistir aparecem ao passar o mouse sobre o vídeo e somem sozinhos.
Clique duplo no vídeo para tela cheia.
Áudio
Transmite somente o som do sistema. O microfone nunca é capturado.
Ao compartilhar a tela inteira, vai o som de todo o sistema.
Ao compartilhar um aplicativo, vai somente o som daquele aplicativo. O resto, como o Discord, fica de fora.
Codec automático e baixo consumo
Ao abrir, o programa testa o seu hardware e escolhe o melhor codec:
NVIDIA (NVENC), AMD (AMF/VCN) e Intel (Quick Sync) são aproveitados por meio do Windows.
A ordem de preferência com aceleração por hardware é AV1, H.265, H.264 e VP9.
Sem aceleração por hardware, o programa usa H.264 por software, que é o mais leve para o processador.
O codec também leva em conta o que o PC de quem assiste decodifica com pouco esforço, para evitar tela preta e uso excessivo de processador.
Na página de ajustes você vê o resultado, por exemplo: `AV1: hardware | H265: hardware | H264: hardware`.
Atualização automática
O programa verifica por versões novas sozinho, baixa em segundo plano e avisa no canto da tela. Basta clicar em Reiniciar e atualizar, ou ele atualiza quando você fecha o programa.
---
Requisitos
Windows 11, ou Windows 10 versão 2004 ou superior, build 20348 ou mais recente (necessário para capturar o som de um aplicativo específico).
Internet. Para transmitir, o upload de quem transmite importa (veja a tabela abaixo).
Não precisa de conta, cadastro ou instalação de outros programas.
Quanto de upload é preciso (para quem transmite)
Cada espectador recebe um fluxo próprio. Valores aproximados a 60 FPS:
Resolução	Bitrate sugerido	1 espectador	5 espectadores
1080p	6 a 8 Mbps	8 Mbps	40 Mbps
720p	3 a 5 Mbps	5 Mbps	25 Mbps
480p e menores	1 a 2 Mbps	2 Mbps	10 Mbps
Se a sua internet não aguentar, reduza o bitrate, a resolução ou o FPS na página de ajustes.
---
Como usar
Criar uma sala
Abra o ScreenLink e digite seu nome.
Clique em Criar nova sala.
Clique em Copiar código e envie para os amigos pelo Discord.
Entrar em uma sala
Digite seu nome e o código de 5 caracteres.
Clique em Entrar na sala.
Transmitir
Dentro da sala, clique em Compartilhar tela.
Escolha a fonte, a resolução, o FPS e o bitrate. Deixe o codec em Automático.
Clique em Iniciar transmissão. Para parar, clique em Parar transmissão.
Assistir
Clique em Assistir ao lado do nome de quem está transmitindo.
Passe o mouse sobre o vídeo para ver volume, ping e o botão de parar.
---
Privacidade e segurança
Vídeo, áudio e chat vão direto entre os participantes e são criptografados (WebRTC).
Um servidor público gratuito (PeerJS) é usado só no começo, para os PCs se encontrarem. Ele não recebe vídeo, áudio nem mensagens do chat.
Se a conexão direta entre dois PCs não for possível, o programa usa um servidor de apoio (relé), por onde o tráfego, ainda criptografado, passa. Nesse caso a qualidade pode cair.
Quem sabe o código da sala pode entrar. Não publique o código em lugares abertos.
O microfone nunca é acessado.
---
Limitações conhecidas
Somente Windows.
Sem conversa por voz. O ScreenLink é um complemento: use o Discord para falar.
Sem histórico no chat. Quem entra depois não vê as mensagens anteriores, e o chat some ao sair da sala.
Máximo de 1080p.
Aplicativos da Microsoft Store (como Calculadora e Filmes e TV) podem ficar sem som ao compartilhar só o aplicativo.
Jogos em tela cheia exclusiva podem aparecer pretos. Use o modo "Janela sem bordas" do jogo ou compartilhe a tela inteira.
Janelas minimizadas não podem ser capturadas.
Depende de um serviço público gratuito para as pessoas se encontrarem. Se ele ficar fora do ar, não é possível criar nem entrar em salas.
Algumas redes (firewalls corporativos, por exemplo) podem impedir a conexão.
---
Problemas comuns
Problema	O que tentar
"Sala não encontrada"	Confira o código e se quem criou a sala ainda está com o programa aberto
"A sala existe, mas a conexão não completou"	A rede ou o firewall está bloqueando. Tente de novo ou use outra rede
Imagem travando ou com baixa qualidade	Reduza o bitrate, a resolução ou o FPS
Sem som na transmissão	Veja se há som tocando e se o dispositivo de saída padrão do Windows está correto
Codec automático não detectou hardware	Na página de ajustes, clique em Detectar hardware de novo
Tela preta ao compartilhar um jogo	Use o modo janela sem bordas ou compartilhe a tela inteira
---
Tecnologias
Aplicativo feito com Electron, comunicação em tempo real com WebRTC (via PeerJS) e um auxiliar nativo para captura de áudio do Windows (WASAPI).
---
Versões
Todas as versões e o histórico estão na página de Releases.
