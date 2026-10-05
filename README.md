# Leandro Jumper Connector — downloads

O **Leandro Jumper Connector** é o programa que liga o iPhone, pelo cabo USB, ao painel do [Leandro Jumper](https://leandrojumper.com.br). Ele roda no seu computador, perto do relógio, e é a ponte entre o cabo e a página: o painel pede, o conector lê o aparelho e devolve os dados.

Este repositório só distribui o instalador. O código fica no repositório da plataforma.

## Baixar

- **Última versão:** [LeandroJumperConnector.exe](https://github.com/xuinda/leandro-jumper-downloads/releases/latest/download/LeandroJumperConnector.exe)
- **Todas as versões e as notas de cada uma:** [Releases](https://github.com/xuinda/leandro-jumper-downloads/releases)

## Requisitos

- Windows 10 ou 11, 64 bits.
- **Driver da Apple instalado.** O conector não traz o driver junto. Instale um destes:
  - o **iTunes**, baixado do site da Apple;
  - o app **Dispositivos Apple** (Apple Devices), da Microsoft Store.

  Para saber se está ok: com o iPhone no cabo e desbloqueado, ele precisa pedir **"Confiar neste computador?"**.

## Como usar

1. Abra o `LeandroJumperConnector.exe`. Não precisa instalar.
2. Ele fica no ícone perto do relógio, às vezes dentro da setinha `^`.
3. Entre no painel em [leandrojumper.com.br](https://leandrojumper.com.br), na tela **Conectar iPhone**, e plugue o aparelho.

## Conferir o arquivo

Cada release traz um `SHA256SUMS.txt`. No PowerShell, na pasta do download:

```powershell
Get-FileHash .\LeandroJumperConnector.exe -Algorithm SHA256
```

O valor tem que ser igual ao do `SHA256SUMS.txt` da mesma versão.

## Aviso do Windows

O executável ainda não tem assinatura digital, então o Windows SmartScreen pode mostrar **"O Windows protegeu o computador"**. Só siga em frente, em **Mais informações → Executar assim mesmo**, se o arquivo veio daqui e o SHA-256 conferiu.
