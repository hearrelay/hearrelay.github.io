---
title: Segurança — HearRelay
lang: pt-BR
---

# Segurança

Obrigado por nos ajudar a manter os usuários do HearRelay em segurança. Esta página explica como reportar vulnerabilidades e resume a postura de segurança do HearRelay.

> Esta tradução é fornecida por conveniência. Em caso de divergência com a [versão em inglês](/en/security/), prevalecerá a versão em inglês.

---

## Reportando uma vulnerabilidade

Envie um e-mail para **hearrelay-security@conex-cp.com** com as seguintes informações:

- Uma descrição clara do problema
- Passos para reproduzir (ou prova de conceito)
- A versão do HearRelay e a versão do iOS / iPadOS utilizadas
- Qualquer mitigação sugerida
- Se você deseja receber crédito público

Preferimos e-mail para o relato inicial. Se necessário, podemos abrir um **GitHub Security Advisory (divulgação privada)** para acompanhar a coordenação.

**Por favor, não divulgue** detalhes de uma vulnerabilidade antes que tenhamos tido a chance de responder e lançar uma correção.

---

## O que consideramos no escopo

Os seguintes itens estão no escopo para relatos:

- O aplicativo HearRelay para iOS / iPadOS
- O handshake criptográfico e o transporte TLS usados entre dispositivos pareados
- O processo de descoberta de pares baseado em iCloud Key-Value Storage
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

| Severidade | Primeira resposta | Resolução alvo |
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

1. **Minimização de dados** — nenhum áudio ou gravação sai do seu dispositivo; nenhum SDK de análise ou publicidade.
2. **Somente rede local** — dispositivos pareados se comunicam exclusivamente pela mesma Wi-Fi / rede local, nunca pela Internet.
3. **Identidade criptográfica do par** — dispositivos se identificam mutuamente com chaves **Curve25519 / P-256**, protegidas no **Secure Enclave** quando disponível, e descobertos via iCloud Key-Value Storage com o escopo da sua Apple ID.

O transporte é criptografado com **TLS 1.3** usando apenas as suítes AEAD fornecidas pelo iOS.

Para uma descrição técnica mais completa, consulte a documentação de design do projeto.

---

## Contato

- Relatos de segurança: **hearrelay-security@conex-cp.com**
- Contato geral: **hearrelay-support@conex-cp.com**

---

**English version:** [Security](/en/security/)
