---
title: Segurança — HearRelay
lang: pt-BR
---

> Esta versão em português é fornecida por conveniência. Em caso de divergência ou discrepância entre esta versão e a versão em inglês, a versão em inglês prevalecerá na medida permitida pela lei aplicável. Esta regra de precedência não limita os direitos que lhe são conferidos por leis imperativas de proteção ao consumidor, privacidade ou proteção de dados.

# Segurança

**Versão do documento: v3.2026-04-26**

Obrigado por nos ajudar a manter os usuários do HearRelay em segurança. Esta página explica como reportar vulnerabilidades e resume a postura de segurança do HearRelay.

---

## Reportando uma vulnerabilidade

Envie um e-mail para **hearrelay-security@conex-cp.com** com as seguintes informações:

- Uma descrição clara do problema
- Passos para reproduzir (ou prova de conceito)
- A versão do HearRelay e a versão do iOS / iPadOS utilizadas
- Qualquer mitigação sugerida que você tenha em mente
- Se você gostaria de receber crédito público

Preferimos e-mail para o relato inicial. Se necessário, podemos abrir um **GitHub Security Advisory (Divulgação Privada)** para a coordenação contínua.

**Por favor, não publique** detalhes de uma vulnerabilidade antes que tenhamos tido a chance de responder e lançar uma correção.

---

## Porto seguro (safe-harbor) para pesquisa de segurança de boa-fé

No momento, não oferecemos um programa de bug bounty nem recompensas monetárias.

Ao testar ou reportar vulnerabilidades, por favor:

- **Não** acesse, modifique, exclua ou exfiltre dados que não sejam seus.
- **Não** realize testes de negação de serviço, spam, phishing, ataques de engenharia social ou qualquer ataque físico.
- **Não** teste contra serviços da Apple, hardware de terceiros ou qualquer sistema que não seja seu.
- Limite os testes aos seus próprios dispositivos e à sua própria Apple ID.

Se você fizer um relato de boa-fé dentro do escopo desta política e cumprir estas regras, **a CONEX não buscará intencionalmente medidas legais contra você baseadas exclusivamente nesse relato**, observada a lei aplicável.

**Limitações importantes.** Esta política **não** autoriza acesso a qualquer sistema, serviço, conta, dispositivo ou dado sem permissão. Ela **não** renuncia nem limita qualquer lei criminal, autoridade regulatória ou direitos de terceiros. Ela **não** vincula a Apple, o GitHub, provedores de e-mail, provedores de nuvem, autoridades policiais, promotores, reguladores ou qualquer outro terceiro.

Poderemos tomar as medidas apropriadas — incluindo notificar partes afetadas ou autoridades — em casos envolvendo extorsão, ameaças, exploração ativa, dano a usuários, acesso não autorizado a sistemas de terceiros ou **descumprimento substancial desta política após notificação, quando o problema puder ser corrigido razoavelmente**.

---

## O que consideramos no escopo

Os seguintes itens estão no escopo para relatos:

- O aplicativo HearRelay para iOS / iPadOS
- O handshake do HearRelay Secure Channel (X25519 ECDH + P-256 ECDSA + AEAD ChaCha20-Poly1305)
- O processo de descoberta de pares baseado no iCloud Key-Value Storage
- O manuseio local de arquivos (armazenamento de gravações e exclusão automática)
- O site do projeto em `hearrelay.app`

---

## Fora do escopo

- Vulnerabilidades nos sistemas operacionais, frameworks ou infraestrutura iCloud da Apple — por favor, reporte diretamente à Apple
- Vulnerabilidades em roteadores Wi-Fi, fones Bluetooth ou outros hardwares de terceiros
- Ataques de engenharia social contra o desenvolvedor ou outros usuários
- Ausência de cabeçalhos de segurança no GitHub Pages além do que a plataforma nos permite configurar
- Problemas que requerem um dispositivo com jailbreak ou de outra forma comprometido

---

## Metas de resposta

| Severidade | Primeira resposta | Resolução-alvo |
|---|---|---|
| Crítica | em até 24 horas | em até 7 dias |
| Alta | em até 3 dias | em até 30 dias |
| Média / Baixa | em até 7 dias | próxima versão regular |

São metas, não garantias.

---

## Divulgação coordenada

- Manteremos você informado durante a investigação.
- Definiremos juntos uma data de divulgação pública, normalmente quando a correção for lançada.
- No lançamento, publicaremos um aviso de segurança e (com sua permissão) daremos crédito a você.

---

## Resumo da postura de segurança

O HearRelay é projetado em torno de três princípios:

1. **Minimização de dados** — áudio e gravações nunca saem do seu dispositivo; sem SDKs de análise ou publicidade.
2. **Somente rede local** — dispositivos pareados se comunicam exclusivamente pela mesma Wi-Fi / rede local, nunca pela Internet.
3. **Identidade criptográfica do par** — os dispositivos se identificam mutuamente com chaves de assinatura **P-256** (armazenadas no **Secure Enclave** quando disponível, com fallback no Keychain) e descobrem-se uns aos outros via iCloud Key-Value Storage no escopo da sua Apple ID.

### Visão geral do fluxo de dados

```text
[Microfone do dispositivo A]
         |
         | apenas processamento local
         v
[App do dispositivo A] <─── canal P2P criptografado na mesma rede Wi-Fi ───> [App do dispositivo B]
         |
         | apenas metadados de descoberta de dispositivo (chave pública, impressão digital,
         | nome do dispositivo, plataforma/modelo, versão do app, datas da chave)
         v
[Apple iCloud Key-Value Storage, escopo do ID Apple]

[Apple App Store + In-App Purchase]   ─── a Apple processa os pagamentos
[Servidor CONEX]                      ─── nenhum
[SDKs de terceiros de análise / publicidade / rastreamento]   ─── nenhum
```

A CONEX não opera nenhum servidor e não tem acesso operacional aos dados armazenados no Apple iCloud nem aos dados processados pelo Apple IAP. Os únicos dados que a CONEX recebe diretamente são os que os usuários enviam voluntariamente por e-mail (veja [Política de Privacidade §4](/pt-BR/privacy/)).

O transporte usa o **HearRelay Secure Channel**: X25519 ECDH para acordo de chaves com sigilo persistente (forward-secret), AEAD ChaCha20-Poly1305 com proteção contra repetição, e nonces derivados de contador por quadro.

Você pode girar a chave de identidade do seu dispositivo, esquecer um dispositivo par ou apagar todo o estado de segurança do dispositivo a qualquer momento em **Ajustes → Segurança** dentro do Aplicativo.

Para uma descrição interna mais completa, consulte a documentação de design do projeto.

---

## Contato

- Relatos de segurança: **hearrelay-security@conex-cp.com**
- Contato geral: **hearrelay-support@conex-cp.com**

---

**Traduções disponíveis em:** [日本語](/ja/security/) · [Français](/fr/security/) · [Español](/es/security/) · [Português (Brasil)](/pt-BR/security/) · [简体中文](/zh-Hans/security/)

Quando esta página for fornecida em qualquer idioma diferente do inglês, a **versão em inglês prevalecerá** na medida permitida pela lei aplicável. Esta regra de precedência não limita os direitos que lhe são conferidos por leis imperativas de proteção ao consumidor, privacidade ou proteção de dados do seu país ou região.
