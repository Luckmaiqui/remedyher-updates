# Luna · Atualizações Android

Canal público de APKs assinados do Luna. Código-fonte, registros pessoais e chaves privadas não são publicados neste canal.

## Instalar

Baixe o APK em [Releases](https://github.com/Luckmaiqui/remedyher-updates/releases/latest) e instale por cima da versão anterior, sem desinstalar.

A partir da versão 1.4, o aplicativo verifica novas releases estáveis, baixa o APK e valida tamanho, SHA-256, pacote e assinatura. O Android controla a instalação e pode pedir autorização ou confirmação. Formulários e ajustes ainda não salvos adiam a instalação.

## Publicar uma atualização

Cada release estável deve incluir `Luna-X.Y.Z.apk` e `update.json`, com a mesma versão, além do arquivo SHA-256. Use o script `tools/publish_release.py` do projeto local para gerar e publicar esses arquivos com a chave de assinatura original. O aplicativo consulta a release publicada diretamente; `latest.json` mantém um espelho para contingência de limite da API.

Não substitua os bytes de uma versão publicada. Aumente `versionCode` e `versionName` para cada atualização.
