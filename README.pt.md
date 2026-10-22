# 📺 DiPlay: CarPlay na tela Android do seu carro (BYD) sem dongle — guia rápido

[![Stars](https://img.shields.io/github/stars/shihabal3amri/DiPlay?style=social)](https://github.com/shihabal3amri/DiPlay/stargazers) ![License](https://img.shields.io/badge/licen%C3%A7a-MIT-green.svg) ![Languages](https://img.shields.io/badge/idiomas-ES%20%C2%B7%20PT-blue)

Apoio e mais: [GitHub Sponsors](https://github.com/sponsors/Ezra-Zhao) · [Gumroad — modelos e cadernos que eu uso](https://ezraflow28.gumroad.com) · [Ko-fi](https://ko-fi.com/ezra777zhao)

> 🌍 [Español](README.md)

Um **guia de uma página só** sobre o **DiPlay**: o app que transforma a tela Android do seu carro em um receptor de CarPlay, com cabo ou sem cabo. Tudo o que você precisa para decidir se ele serve para você e fazer a conexão: compatibilidade real, os dois métodos de conexão em três passos e os avisos que o próprio projeto faz.

**Autor:** Ezra-Zhao · Outubro de 2026

Projeto original: https://github.com/shihabal3amri/DiPlay · Downloads: https://github.com/shihabal3amri/DiPlay/releases · Site: https://shihabal3amri.github.io/DiPlay/

> **Nota de autoria:** este é um guia original de síntese, escrito com palavras próprias a partir da documentação pública do projeto; não reproduz o texto dele. A compatibilidade citada é a que o projeto declara no seu README e no documento de compatibilidade (versão 0.2.21, prévia pública).

---

## Em 20 segundos

- O DiPlay é instalado **no carro** (na tela Android), **não no iPhone**.
- **Sem dongle, sem jailbreak, sem Mac, sem conta e sem servidor de autenticação.** A autenticação do CarPlay é local.
- Funciona **com cabo USB** ou **sem fio**: Wi-Fi Direct, o hotspot do próprio carro ou a mesma rede Wi-Fi/LAN.
- O projeto é **focado na BYD (DiLink)**. Em outras marcas pode funcionar, mas o autor declara que elas não têm suporte.
- É uma **prévia pública** (0.2.21), não um produto acabado nem certificado.

## Compatibilidade (o que foi verificado, direto ao ponto)

| Peça | O que o projeto diz |
|---|---|
| Sistema da tela | Android **7.0+ (API 24)** para instalar o APK. **Android 6.0 ou anterior: não é compatível.** |
| Condição prévia | A central multimídia **precisa permitir a instalação de APKs**. Sem isso, nada do restante se aplica. |
| Android 7.0–8.1 | O APK instala, mas o projeto indica que **ainda não foi confirmado em um veículo real**. |
| Alcance principal | Carros **BYD com DiLink**. Evidências citadas pelo projeto: carro de desenvolvimento com DiLink 5.1, um BYD Tang com DiLink 5.0 e instalação do zero validada em DiLink 4.0 / Android 10. |
| Outras marcas | **Sem suporte oficial**: o projeto é focado na BYD e não promete corrigir incompatibilidades de outras marcas. Há relatos mistos da comunidade entre gerações do DiLink; **não existe uma lista certificada de modelos**. |
| iPhone | iPhone comum, **sem jailbreak**, com o CarPlay ativado. A compatibilidade exata varia conforme o modelo e o iOS. |
| Sem fio | Wi-Fi Direct, hotspot do carro ou Wi-Fi existente / mesma LAN. No **Android 7.0–9**, o Wi-Fi Direct usa um caminho legado que **depende do firmware**; no **Android 10+** a frequência negociada do grupo é verificada. |
| Recomendação do projeto | O **hotspot integrado do carro** é a conexão recomendada: com Wi-Fi Direct, a busca de redes do próprio carro pode causar microcortes no áudio. |
| Porta USB | Precisa ser uma porta **de dados**. Uma porta só de carga não transmite nada e a conexão não inicia. |
| ADB | **Não é necessário** para o CarPlay básico. Só é pedido por funções opcionais (painel, bateria, velocidade das rodas, vídeo com o carro parado). |

## Conexão com cabo (3 passos)

1. **Instale o DiPlay na tela do carro**: baixe o APK na página de *Releases* do projeto e permita a instalação de APK na central.
2. **Conecte o iPhone a uma porta USB de dados** do carro com o próprio cabo USB.
3. **Abra o DiPlay e escolha o CarPlay com cabo**: a autenticação é local e a sessão começa na tela.

## Conexão sem fio (3 passos)

1. **Instale o DiPlay na tela** (como acima) e abra o app.
2. **Ative o hotspot do carro** (a opção recomendada) ou o Wi-Fi Direct na tela. Atenção: no Android 7–9, o Wi-Fi Direct depende do firmware de cada unidade.
3. **Conecte o iPhone a esse hotspot ou rede** e escolha o CarPlay sem fio no DiPlay; deixe a conexão automática a esse hotspot ativada para reconectar sozinho.

## Avisos honestos (leia antes de instalar)

- **Não é um produto certificado pela Apple.** Sem afiliação nem endosso da Apple ou da BYD: CarPlay é marca da Apple e o projeto a usa apenas para descrever a função.
- **Identidade de acessório experimental:** o APK inclui uma identidade recuperada de firmware público da Carlinkit; não é uma identidade MFi nova criada para o DiPlay, e a chave privada incluída pode ser extraída. Não há garantia de que versões futuras do iOS continuem a aceitá-la.
- **Prévia pública:** pode haver cortes de áudio e comportamentos diferentes conforme o firmware. O próprio projeto pede testes na versão atual e relatórios com a ferramenta de diagnóstico dele.
- **Outras marcas = terreno não verificado:** fora da BYD, se algo falhar, o projeto declara que não há suporte nem planos de adicioná-lo.
- **Antes de perder uma tarde:** confirme primeiro se a sua central permite instalar APK e se você tem uma porta USB de dados; são os dois bloqueios mais comuns.

## Links

- Projeto original: https://github.com/shihabal3amri/DiPlay
- Downloads (Releases): https://github.com/shihabal3amri/DiPlay/releases
- Documento de compatibilidade do projeto: https://github.com/shihabal3amri/DiPlay/blob/main/docs/COMPATIBILITY.md
- Site do projeto: https://shihabal3amri.github.io/DiPlay/

## Licença

Este guia é publicado sob a licença MIT (© 2026 Guangyi Zhao). O DiPlay é um projeto independente do seu autor, sob a licença GPL-3.0; este guia não faz parte desse projeto nem o substitui: para instalar, use sempre os links oficiais acima.
