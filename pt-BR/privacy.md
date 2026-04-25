---
title: Política de Privacidade — HearRelay
lang: pt-BR
---

> Esta versão em português é fornecida por conveniência. Em caso de divergência ou discrepância entre esta versão e a versão em inglês, a versão em inglês prevalecerá na medida permitida pela lei aplicável. Esta regra de precedência não limita os direitos que lhe são conferidos por leis imperativas de proteção ao consumidor, privacidade ou proteção de dados.

# Política de Privacidade

**Data de vigência: 25 de abril de 2026**
**Última atualização: 26 de abril de 2026**
**Versão do documento: v3.2026-04-26**

## Resumo

O HearRelay foi projetado para funcionar sem um servidor de back-end da CONEX. O áudio e as gravações permanecem em seus dispositivos. Os metadados de descoberta de dispositivos são armazenados apenas no Apple iCloud dentro do escopo do seu ID Apple. Os pagamentos são processados pela Apple. A CONEX recebe informações pessoais somente se você optar por nos contatar por e-mail — consulte §4 para detalhes.

---

O HearRelay (o "Aplicativo") foi projetado para ser privado por padrão. Esta política explica quais dados são, e quais não são, tratados quando você usa o HearRelay.

Se tiver alguma dúvida, entre em contato conosco pelo e-mail **hearrelay-privacy@conex-cp.com**.

---

## 1. Quem somos

O HearRelay é desenvolvido pela **CONEX Corporation** (株式会社CONEX), empresa constituída no Japão (o "Desenvolvedor", "nós", "nossa", "CONEX"). O Aplicativo é projetado de forma que áudio, gravações, informações de pagamento, identificadores publicitários, dados analíticos e dados de rastreamento não sejam transmitidos a servidores da CONEX. A CONEX não opera qualquer servidor de back-end para o Aplicativo.

Na medida em que qualquer informação limitada de descoberta de dispositivo seja tratada pela Apple dentro da sua conta ID Apple (consulte o §5), a CONEX não acessa nem opera tal tratamento. Quando a lei aplicável, ainda assim, tratar tais informações como "dados pessoais", a CONEX coopera de boa-fé com solicitações de informação nos termos do §12.

Se você optar por entrar em contato conosco por e-mail — para suporte, privacidade, segurança ou outras consultas —, a CONEX receberá o conteúdo desses e-mails (consulte o §4).

Para correspondência, utilize os endereços de e-mail no final desta página.

---

## 2. Dados que não coletamos por meio do Aplicativo

Exceto pelas informações que você optar por nos enviar diretamente (consulte o §4), a CONEX **não** coleta nem recebe em seus próprios servidores, não armazena nem compartilha nenhum dos seguintes dados por meio do Aplicativo:

- Áudio captado pelo microfone do seu dispositivo
- Gravações de áudio criadas por você com o Aplicativo
- Informações de contato, localização, fotos, dados da câmera ou identificadores de dispositivo
- Identificadores publicitários (IDFA, IDFV usados para rastreamento)
- Dados analíticos, telemetria de falhas encaminhada a serviços de terceiros, ou perfis comportamentais
- Dados de cartão de pagamento ou de cobrança (a Apple processa as compras — consulte o §8)

O HearRelay não contém quaisquer SDKs de terceiros para análises, publicidade ou rastreamento.

---

## 3. Dados tratados localmente no seu dispositivo

O Aplicativo trata os seguintes dados no seu dispositivo, e **apenas no seu dispositivo**:

| Dado | Finalidade | Retenção |
|---|---|---|
| Áudio do microfone (ao vivo) | Monitoramento em tempo real para fones de ouvido ou para um dispositivo pareado na mesma rede Wi-Fi | Não armazenado |
| Gravações de áudio (opcional) | Você pode gravar sessões manualmente | Excluídas automaticamente após 24 horas, por padrão; você pode estender o prazo ou excluí-las antes |
| Histórico de conexão (nome do par, data da última conexão) | Recurso de conveniência para reconectar rapidamente | Armazenado localmente; removido ao desinstalar o Aplicativo |
| Preferências do Aplicativo (incluindo a data de início do período de avaliação para controle de compra) | Lembrar suas configurações | Armazenadas localmente |

Quando você desinstala o Aplicativo, todos os dados acima são removidos com ele.

---

## 4. Comunicações que você nos envia

O Aplicativo é projetado de modo que a CONEX não colete nem receba dados pessoais por meio do Aplicativo em seus próprios servidores.

No entanto, se você optar por entrar em contato com a CONEX por e-mail para suporte, solicitações de privacidade, relatos de segurança, dúvidas relacionadas a reembolsos ou outras consultas, **receberemos as informações que você optar por enviar**. Isso pode incluir:

- Seu endereço de e-mail
- Seu nome, se incluído na sua mensagem
- O conteúdo da sua mensagem
- Modelo do dispositivo, versão do iOS / iPadOS, versão do aplicativo
- Capturas de tela, registros (logs), passos de reprodução
- Detalhes de vulnerabilidade (em relatos de segurança)

**Finalidade.** A CONEX usa essas informações apenas para responder à sua consulta, prestar suporte, investigar questões de segurança, cumprir obrigações legais e proteger o Aplicativo e nossos usuários. **Não** usamos correspondência de suporte, privacidade ou segurança para publicidade, rastreamento ou perfilamento.

**Prestadores de serviços.** Essas comunicações podem ser tratadas por nossos prestadores de serviços de e-mail, hospedagem ou recebimento de relatos de segurança. Dependendo do prestador, as informações podem ser armazenadas ou tratadas no Japão ou em outros países.

**Retenção.** Mantemos a correspondência apenas pelo tempo razoavelmente necessário para a finalidade para a qual foi fornecida. Em geral:

- **consultas de suporte**: até **30 dias** após o encerramento do caso;
- **solicitações relativas a direitos de privacidade**: até **3 anos** após a conclusão da solicitação, para manutenção de registros de conformidade;
- **relatórios de vulnerabilidades de segurança**: até **2 anos** após a conclusão da correção ou versão correspondente;
- **reivindicações jurídicas, fraude, extorsão, abuso ou questões com autoridades**: pelo período razoavelmente necessário para proteger direitos legais, cumprir obrigações legais, resolver disputas ou cooperar com solicitações lícitas.

Podemos excluir informações antes quando não forem mais necessárias, e podemos manter registros limitados por mais tempo quando a lei aplicável exigir ou permitir.

---

## 5. Informações limitadas tratadas pelo Apple iCloud (escopo da ID Apple)

Para permitir que seus próprios dispositivos Apple se encontrem na mesma rede Wi-Fi, o Aplicativo faz com que as seguintes informações limitadas de descoberta de dispositivo sejam armazenadas no **Apple iCloud Key-Value Storage**, dentro da sua conta ID Apple:

- Uma **chave pública** criptográfica gerada no seu dispositivo
- Uma **impressão digital SHA-256** dessa chave pública
- O **nome** do seu dispositivo (conforme definido em Ajustes do iOS → Geral → Sobre → Nome)
- A **plataforma**, o **modelo** do seu dispositivo, e a **versão do aplicativo** instalada
- A **data de criação** e a **data da última rotação** da chave

Essas informações são armazenadas no escopo da sua própria ID Apple, dentro do serviço iCloud da Apple, e não são visíveis para outros titulares de ID Apple nem para a CONEX. A CONEX não opera o Apple iCloud e não acessa essas informações em seus próprios servidores. O tratamento pela Apple é regido pela política de privacidade da própria Apple e pelos termos do iCloud.

**Dependendo da lei aplicável e das configurações do nome do seu dispositivo, algumas dessas informações podem ser consideradas dados pessoais** — por exemplo, se o nome do seu dispositivo contiver seu nome completo. Descrevemo-las aqui por transparência. Você pode alterar o nome do seu dispositivo a qualquer momento nos Ajustes do iOS, e pode purgar a identidade do Aplicativo (girando sua chave e apagando a entrada) em **Ajustes → Segurança → Redefinir toda a segurança do dispositivo** dentro do Aplicativo.

---

## 6. Comunicação em rede

O HearRelay se comunica **apenas** com outros dispositivos Apple que estejam:

1. Conectados à **mesma ID Apple**, **e**
2. Conectados à **mesma rede Wi-Fi / rede local**

A comunicação é criptografada com o **HearRelay Secure Channel** (acordo de chaves X25519 ECDH + AEAD ChaCha20-Poly1305 com proteção contra repetição). O HearRelay **não** envia quaisquer dados pela Internet para servidores remotos, nem oferece suporte a monitoramento remoto entre redes. O uso remoto é deliberadamente proibido para evitar vigilância clandestina.

---

## 7. Gravações de áudio que você cria

Se você ativar o recurso de gravação:

- As gravações são salvas **apenas no dispositivo que as criou**
- As gravações são armazenadas dentro do sandbox do Aplicativo com **criptografia em nível de arquivo** (`NSFileProtectionComplete`)
- As gravações são **excluídas automaticamente 24 horas** após a criação, salvo se você escolher explicitamente preservá-las
- Você pode compartilhar ou exportar gravações por meio da folha de compartilhamento do iOS, sob seu controle
- As gravações nunca são enviadas pelo Aplicativo à CONEX nem a terceiros

Você é responsável por confirmar que qualquer gravação ou monitoramento ao vivo que realize cumpra todas as leis aplicáveis — incluindo exigências de consentimento que possam aplicar-se ao seu local. Consulte nossos [Termos de Uso](/pt-BR/terms/) e a página de [Suporte](/pt-BR/support/) para mais informações.

---

## 8. Terceiros, pagamentos e a App Store

- A CONEX **não** vende, aluga nem compartilha dados pessoais para fins de publicidade, análises ou rastreamento. Os serviços da Apple e as comunicações voluntárias que você nos envia estão descritos nesta Política (consulte os §4 e §5).
- O Aplicativo **não** utiliza SDKs de publicidade, análises ou perfilamento.

A distribuição e os pagamentos são realizados pela Apple por meio da App Store e da Compra no Aplicativo (In-App Purchase). **O HearRelay Full Access é uma compra única, do tipo Não-Consumível, e não uma assinatura com renovação automática.** Preços, impostos, reembolsos e cobranças são processados pela Apple sob os Termos da App Store e dos Apple Media Services. A CONEX não recebe números de cartão de pagamento nem detalhes de cobrança. Você pode restaurar uma compra anterior usando a opção **Restore Purchases** dentro do Aplicativo.

Quando a Apple processa sua compra ou entrega atualizações, a política de privacidade da própria Apple se aplica a essa atividade. Quaisquer informações de diagnóstico que a Apple coletar do seu dispositivo (por exemplo, registros de falhas enviados via "Compartilhar com Desenvolvedores de Apps") são regidas pelos Ajustes do iOS e pelos termos para desenvolvedores da Apple.

---

## 9. Nosso site

O site do HearRelay em <https://hearrelay.app/> é um site informacional estático hospedado no GitHub Pages. **Não** utilizamos cookies publicitários, cookies analíticos, pixels de rastreamento ou tags de marketing de terceiros.

Como ocorre com a maioria dos sites hospedados, o GitHub ou os provedores de infraestrutura podem tratar registros técnicos padrão, tais como endereços IP e metadados de requisição, para entregar e proteger o site. A CONEX não utiliza esses registros para publicidade, análises ou rastreamento.

Caso nosso uso do site mude de forma material, atualizaremos esta Política e forneceremos quaisquer avisos ou opções exigidos pela lei aplicável.

---

## 10. Usuários internacionais

Como o HearRelay não transfere dados dos seus dispositivos para servidores da CONEX, não há transferência internacional de dados pessoais realizada pela CONEX. A correspondência voluntária por e-mail pode ser tratada por prestadores de serviços conforme descrito no §4.

### 10.1 Usuários no Espaço Econômico Europeu (EEE), Reino Unido e Suíça

O Aplicativo é projetado de modo que a CONEX não colete nem receba em seus próprios servidores áudio, gravações, informações de pagamento, dados analíticos, identificadores publicitários ou dados de rastreamento.

Informações limitadas de descoberta de dispositivo podem ser armazenadas no Apple iCloud, dentro da sua conta ID Apple (§5). A CONEX não opera o Apple iCloud e não acessa essas informações em seus próprios servidores.

Na medida em que a CONEX seja considerada controladora desse tratamento limitado, as **finalidades** do tratamento são permitir descoberta de dispositivos, autenticação mútua, segurança e comunicação local ponto-a-ponto entre seus próprios dispositivos.

As **bases legais** são:

- **execução do contrato** da licença do aplicativo e de serviços relacionados solicitados por você, para permitir descoberta de dispositivos, autenticação e comunicação local ponto-a-ponto (**Artigo 6(1)(b) do GDPR**); e
- os **interesses legítimos** da CONEX na manutenção da segurança, integridade, prevenção de abusos e arquitetura de rede local preservadora de privacidade do Aplicativo (**Artigo 6(1)(f) do GDPR**).

Quando a lei aplicável exigir consentimento para uma operação específica, **solicitaremos seu consentimento antes dessa operação e o utilizaremos como base** (**Artigo 6(1)(a) do GDPR**). Você pode retirar esse consentimento desativando o iCloud para o Aplicativo, redefinindo as configurações de segurança do dispositivo no Aplicativo ou desinstalando o Aplicativo, embora isso possa impedir o funcionamento da descoberta de dispositivos ou do pareamento.

Para a **correspondência voluntária por e-mail** (§4), as bases legais são a execução de qualquer obrigação de suporte, pré-contratual ou contratual solicitada por você (**Artigo 6(1)(b) do GDPR**), e os interesses legítimos da CONEX em responder a consultas e manter a segurança do Aplicativo (**Artigo 6(1)(f) do GDPR**).

**Representante na UE.** A CONEX não designou atualmente um representante no EEE. Com base na avaliação atual da CONEX, o Aplicativo é projetado de modo que a CONEX não coleta dados pessoais em seus próprios servidores, e qualquer tratamento pelo qual a CONEX possa ser considerada responsável é limitado, de baixo risco e relacionado à descoberta local de dispositivos e à segurança. Reavaliaremos essa posição se nossas atividades de tratamento, base de usuários, regiões de distribuição, orientações aplicáveis ou expectativas regulatórias mudarem de forma material. Isso não limita seu direito de nos contatar em **hearrelay-privacy@conex-cp.com** ou de apresentar reclamação a uma autoridade de supervisão competente.

### 10.2 Usuários no Brasil

A postura de tratamento do App sob a LGPD reflete a do §10.1. A CONEX não tem conhecimento de dados pessoais tratados em seus próprios servidores, exceto correspondência voluntária por e-mail (§4).

**Encarregado / DPO.** A CONEX não nomeou um Encarregado (DPO) local com base em sua avaliação atual de que:

- o App é projetado de modo que áudio, gravações, informações de pagamento, dados analíticos, identificadores publicitários e dados de rastreamento não são transmitidos aos servidores da CONEX;
- os únicos dados pessoais que a CONEX recebe diretamente são a correspondência voluntária por e-mail (§4), tratados em volumes limitados para finalidades de atendimento de solicitações, segurança e conformidade;
- nenhum tratamento de dados pessoais em larga escala, de alto risco ou de categorias especiais ocorre por meio da CONEX.

Esta determinação está documentada internamente e é reavaliada quando nosso volume de tratamento, regiões de distribuição, orientações aplicáveis ou expectativas regulatórias mudarem materialmente. O contato abaixo serve como ponto de contato para solicitações LGPD, incluindo direitos de titulares e consultas da ANPD:

- **E-mail (consultas em português são aceitas; resposta em português ou inglês conforme disponibilidade)**: hearrelay-privacy@conex-cp.com

Se sua consulta se refere especificamente a direitos LGPD, indique "LGPD" no assunto para que possamos priorizar a resposta.

### 10.3 Usuários no Japão

A CONEX não inclui SDKs de publicidade, análise ou rastreamento de terceiros no Aplicativo, e não transmite informações relacionadas a usuários para seus próprios servidores. O Apple iCloud Key-Value Storage é usado exclusivamente para sincronizar as informações limitadas de descoberta de dispositivo descritas no §5 dentro da sua própria conta ID Apple; a CONEX não recebe essas informações em seus próprios servidores.

Esta divulgação é fornecida por transparência e para a avaliação voluntária pela CONEX das regras japonesas de notificação de transmissão externa previstas na Lei de Negócios de Telecomunicações. A CONEX não utiliza SDKs de publicidade, análise ou rastreamento de terceiros, e não recebe essas informações em seus próprios servidores.

### 10.4 Usuários em Hong Kong / Taiwan

A mesma postura de tratamento se aplica. A CONEX está ciente de que a PDPO (Hong Kong) e a Lei de Proteção de Informações Pessoais (Taiwan) definem dados pessoais e informações pessoais de forma ampla; consulte os §5 e §12 para nossa posição e os direitos que você pode exercer.

---

## 11. Privacidade de crianças

O HearRelay é um utilitário destinado a adultos, normalmente pais ou responsáveis. **Não é direcionado a crianças menores de 13 anos**, e a CONEX não coleta intencionalmente dados pessoais de crianças. O tratamento do Aplicativo ocorre localmente no seu dispositivo, portanto nenhum dado pessoal de crianças é coletado, armazenado ou transmitido à CONEX.

---

## 12. Seus direitos

Para os dados que não temos (§2), normalmente não há nada para acessarmos, corrigirmos, excluirmos, exportarmos ou restringirmos. Para a correspondência voluntária por e-mail que recebemos (§4), e na medida em que a lei aplicável trate as informações de descoberta de dispositivo no escopo do Apple iCloud (§5) como seus dados pessoais, dependendo da sua localização (EEE, Reino Unido, Califórnia, Brasil, Japão, Hong Kong, Taiwan etc.), você pode ter direitos legais, incluindo:

- Direito de acesso
- Direito à retificação
- Direito à exclusão
- Direito de se opor ou de restringir o tratamento
- Direito à portabilidade dos dados
- Direito de optar por não ser objeto de "venda" ou "compartilhamento" — a CONEX não vende nem compartilha dados pessoais
- Direito de apresentar reclamação à autoridade de supervisão local

Para exercer qualquer direito, entre em contato em **hearrelay-privacy@conex-cp.com**. Observe que, para excluir todos os dados que o Aplicativo armazenou localmente, basta desinstalar o Aplicativo do seu dispositivo. Para purgar a identidade por dispositivo do Aplicativo no Apple iCloud (§5), use **Ajustes → Segurança → Redefinir toda a segurança do dispositivo** dentro do Aplicativo.

---

## 13. Segurança

### Visão geral do fluxo de dados

```text
[Microfone do dispositivo A]
         |
         | apenas processamento local
         v
[App do dispositivo A] <─── canal P2P criptografado na mesma rede Wi-Fi ───> [App do dispositivo B]
         |
         | apenas metadados de descoberta de dispositivo (veja §5)
         v
[Apple iCloud Key-Value Storage, escopo do ID Apple]

[Apple App Store + In-App Purchase]   ─── a Apple processa os pagamentos
[Servidor CONEX]                      ─── nenhum
[SDKs de terceiros de análise / publicidade / rastreamento]   ─── nenhum
```

### Proteções técnicas

- **HearRelay Secure Channel** (X25519 ECDH + AEAD ChaCha20-Poly1305) para toda a comunicação dispositivo-a-dispositivo
- Chaves de identidade **P-256** geradas e armazenadas no **Secure Enclave** quando disponível, com fallback no Keychain
- **Fixação de chave pública (public-key pinning)** por meio de uma lista de confiança no escopo do iCloud, para impedir que dispositivos impostores se conectem
- **Proteção de arquivos** (`NSFileProtectionComplete`) para gravações locais

Nenhum método de transmissão ou armazenamento é perfeitamente seguro. Para relatar uma vulnerabilidade, consulte nossa [página de Segurança](/pt-BR/security/) e envie um e-mail para **hearrelay-security@conex-cp.com**.

---

## 14. Alterações a esta política

Podemos revisar esta Política de Privacidade. A data da revisão será atualizada no topo desta página, e alterações materiais serão anunciadas nas notas de versão do Aplicativo. Quando a lei aplicável exigir, obteremos seu consentimento ou forneceremos um aviso prévio razoável e uma oportunidade significativa para você deixar de usar o Aplicativo antes que a alteração entre em vigor.

---

## 15. Contato

- Privacidade: **hearrelay-privacy@conex-cp.com**
- Suporte: **hearrelay-support@conex-cp.com**
- Segurança: **hearrelay-security@conex-cp.com**
- Web: <https://hearrelay.app/>

---

**Traduções disponíveis em:** [日本語](/ja/privacy/) · [Français](/fr/privacy/) · [Español](/es/privacy/) · [Português (Brasil)](/pt-BR/privacy/) · [简体中文](/zh-Hans/privacy/)

Quando esta Política for fornecida em qualquer idioma diferente do inglês, a **versão em inglês prevalecerá** na medida permitida pela lei aplicável. Esta regra de precedência não limita os direitos que lhe são conferidos por leis imperativas de proteção ao consumidor, privacidade ou proteção de dados do seu país ou região.
