# UML-iphone
Diagrama de classes para Iphone

```mermaid
classDiagram
  class iPhone {
    + reprodutorMusical: ReprodutorMusical
    + aparelhoTelefonico: AparelhoTelefonico
    + navegadorInternet: NavegadorInternet
  }

  interface ReprodutorMusical {
    + tocarMusica()
    + pausarMusica()
    + ajustarVolume(volume: int)
  }

  interface AparelhoTelefonico {
    + fazerLigacao(numero: string)
    + receberLigacao()
    + enviarMensagem(mensagem: string, numero: string)
  }

  interface NavegadorInternet {
    + abrirPagina(url: string)
    + fecharPagina()
    + navegar(url: string)
  }

  iPhone --> ReprodutorMusical
  iPhone --> AparelhoTelefonico
  iPhone --> NavegadorInternet

```
