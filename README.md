# FDP

Cliente FTP/FTPS nativo para macOS. Dois painéis lado a lado, estilo Finder: o seu Mac de um lado, o servidor do outro. Arrasta e pronto.

Feito por quem cansou dos clientes FTP que existem para Mac.

## Download

A versão mais recente está em [Releases](../../releases/latest). Baixe o `.dmg`, abra e arraste o FDP para a pasta Aplicativos.

Na primeira abertura o macOS pode avisar que o app é de "desenvolvedor não identificado". Clique com o botão direito no FDP, escolha **Abrir** e confirme. Só precisa fazer isso uma vez.

Requer macOS 14 (Sonoma) ou mais novo.

## O que ele faz

- FTP e FTPS (TLS explícito), com TLS ligado por padrão.
- Dois painéis espelhados, com identificação clara de qual é o Mac e qual é o servidor.
- Arrastar e soltar entre os painéis e do Finder para o servidor.
- Fila de transferências visível: progresso, velocidade, cancelar, e pergunta antes de sobrescrever.
- Favoritos com senha guardada só no Keychain do macOS, protegida por Touch ID.
- Nova pasta, renomear e apagar nos dois lados. Apagar no Mac vai para o Lixo.
- Menu, toolbar e botão direito com as mesmas ações.

## Segurança

- O certificado do servidor é validado pelo próprio macOS (confiança do sistema e do seu Keychain).
- O canal de dados reutiliza a sessão TLS do canal de controle, como os servidores FTPS exigem.
- O app nunca conecta em um endereço anunciado pelo servidor: só no host que você digitou.
- Senha nunca é gravada em arquivo. Só no Keychain, e só se você pedir.
- Nada é sobrescrito nem apagado sem você confirmar.

## Código

O FDP é um software proprietário e gratuito. O código-fonte não é público. Este repositório existe só para distribuir as versões.

Problemas e sugestões: abra uma [issue](../../issues).
