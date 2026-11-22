# Floating Cue

Teleprompter flutuante para Chrome no computador (com acompanhamento por voz) e Safari no iPhone (com rolagem por velocidade). No Chrome, o modo voz renderiza a janela Picture in Picture ao vivo, sem gerar MP4.

**Abrir:** https://thiagovitezi.github.io/floatingcue/ (preferencialmente Chrome atualizado no desktop)

- Velocidade ajustável na hora, sem gerar o vídeo de novo
- Tamanho da letra, formato da janela (16:9, 4:3, 1:1, 3:4) e espelhamento
- Contagem 3-2-1, linha de leitura e barra de progresso no vídeo
- Calibragem da velocidade pelo seu ritmo de leitura
- Na janela flutuante: pausar, voltar/avançar 15 s e redimensionar com pinça

O roteiro e as configurações ficam salvos só no aparelho (localStorage).

## Modo voz no Chrome desktop

1. Abra a página no Chrome e cole seu roteiro.
2. Em **Controles > COMO O TEXTO AVANÇA?**, selecione **Por voz · acompanha minhas palavras**.
3. Clique em **Ativar microfone e acompanhar fala** e permita acesso ao microfone do Chrome.
4. Clique em **Abrir janela flutuante** e posicione-a por cima do OBS ou outro programa. Se necessário, pode abrir primeiro o PiP e então ativar o microfone pela página.
5. Fale normalmente. O reconhecimento de fala pt-BR tenta alinhar o que você diz às palavras do roteiro e atualiza o quadro do PiP. Enquanto você não fala, a posição permanece parada.

O modo por voz usa a Web Speech API do Chrome (conforme disponibilidade do navegador e serviço de reconhecimento) e necessita de microfone e conexão de rede. **Não é necessário gerar MP4** nesse modo. A gravação pelo OBS continua independente. A página do Floating Cue deve ficar aberta enquanto você grava.

Para o modo de rolagem por tempo, selecione **Automático · por velocidade** e use **Gerar vídeo do roteiro** como anteriormente.

**Limitações:** o reconhecimento pode falhar com ruído, palavras diferentes do roteiro, falhas de rede ou permissões bloqueadas. O modo voz está implementado, mas precisa de validação com Chrome + microfone + OBS em uma máquina real. No iPhone, o navegador pode suspender o microfone ao alternar para a câmera de outro app.
