# Floating Cue

Teleprompter flutuante para iPhone que roda no Safari. O roteiro vira um vídeo MP4 gerado no próprio aparelho e abre na janela Picture in Picture do iOS, por cima de qualquer app de câmera.

**Abrir:** https://thiagovitezi.github.io/floatingcue/ (no Safari do iPhone, iOS 17+)

- Velocidade ajustável na hora, sem gerar o vídeo de novo
- Tamanho da letra, formato da janela (16:9, 4:3, 1:1, 3:4) e espelhamento
- Contagem 3-2-1, linha de leitura e barra de progresso no vídeo
- Calibragem da velocidade pelo seu ritmo de leitura
- Na janela flutuante: pausar, voltar/avançar 15 s e redimensionar com pinça

O roteiro e as configurações ficam salvos só no aparelho (localStorage).

## Acompanhamento por voz (experimental)

Em **Controles > Avanço do texto**, escolha **Pelas palavras que eu falar**. Gere o vídeo do roteiro e toque em **Ativar microfone e acompanhar fala**. Autorize o microfone e leia em português brasileiro. O sistema tenta encontrar as palavras ditas no roteiro e posicionar o vídeo no trecho correspondente, sem avançar sozinho durante o silêncio.

O modo **Por velocidade** continua disponível. O reconhecimento usa a API de fala do navegador, quando suportada, e pode depender do serviço de reconhecimento oferecido pelo próprio navegador.

**Limitação importante no iPhone:** ao sair do Safari para gravar com a Câmera, Instagram ou outro app, o iOS pode interromper a captura de microfone do Safari. Portanto, o modo por voz não é garantido na janela flutuante enquanto outro app grava. Nessa situação, use a rolagem por velocidade ou teste o projeto nativo [FloatingCue-iOS](https://github.com/ThiagoVitezi/FloatingCue-iOS), cujo modo por voz também é experimental. O reconhecimento por voz foi incluído no código, mas ainda precisa ser validado no Safari de um iPhone real.
