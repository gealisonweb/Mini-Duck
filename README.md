# Mini Duck

Mini Duck é um navegador Android leve para quem usa um celular com pouca memória ou um processador antigo e quer reduzir os dados de navegação que ficam no aparelho. Ele abre direto na busca HTML do DuckDuckGo, com fundo preto AMOLED na pesquisa e nos resultados.

## Por que ele é leve?

O app usa uma única WebView do Android. Foi escrito em Java e não inclui um motor de navegador próprio, bibliotecas externas de execução, serviços em segundo plano ou menus. JavaScript e imagens continuam habilitados. A versão 1.9 com ícone ocupa cerca de 36 KB; o uso de memória e bateria varia conforme o aparelho e as páginas abertas.

## Privacidade no aparelho

O app pede apenas a permissão de internet e não inclui código de telemetria. O botão Voltar usa o histórico da sessão atual. Ao sair do primeiro plano, o navegador encerra a sessão, descarta a WebView e solicita a limpeza de cookies, cache, histórico, dados de formulários e armazenamento web.

A limpeza é local. O DuckDuckGo e os sites visitados ainda recebem as conexões, e a navegação não é anônima. Os downloads são gerenciados pelo Android e os arquivos baixados permanecem na pasta Downloads.

## Compatibilidade e compilação

Android 8.0 ou superior. O app depende da WebView do sistema. Para compilar, use JDK 17 e Android SDK 35.

```powershell
.\gradlew.bat :cru:assembleDebug
```

O APK de teste sai em `cru/build/outputs/apk/debug/`.
