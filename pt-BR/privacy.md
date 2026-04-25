---
title: Política de Privacidade — HearRelay
lang: pt-BR
---

> Esta versão em português é fornecida por conveniência. Em caso de divergência ou discrepância entre esta versão e a versão em inglês, a versão em inglês prevalecerá na medida permitida pela lei aplicável. Esta regra de precedência não limita os direitos que lhe são conferidos por leis imperativas de proteção ao consumidor, privacidade ou proteção de dados.

# Política de Privacidade

**Data de vigência: 2026-04-25**
**Última atualização: 2026-04-25**

O HearRelay (o "Aplicativo") foi projetado para ser privado por padrão. Esta política explica quais dados são, e quais não são, processados quando você usa o HearRelay.

Se tiver alguma dúvida, entre em contato conosco pelo e-mail **hearrelay-privacy@conex-cp.com**.

---

## 1. Quem somos

O HearRelay é desenvolvido pela **CONEX Corporation** (株式会社CONEX), uma empresa constituída no Japão (o "Desenvolvedor", "nós", "nossa", "CONEX"). O Aplicativo é projetado de forma que áudio, gravações, informações de pagamento, identificadores publicitários, dados analíticos e dados de rastreamento não sejam transmitidos a servidores da CONEX. A CONEX não opera qualquer servidor de back-end para o Aplicativo.

Na medida em que qualquer informação limitada de descoberta de dispositivo seja processada pela Apple dentro da sua conta Apple ID (consulte o §4), a CONEX não acessa nem opera tal processamento. Quando a lei aplicável, ainda assim, tratar tais informações como "dados pessoais", a CONEX coopera de boa-fé com solicitações de informação nos termos do §10.

Para correspondência, utilize os endereços de e-mail no final desta página.

---

## 2. Dados que não coletamos

A CONEX **não** coleta nem recebe em seus próprios servidores, não armazena nem compartilha nenhum dos seguintes dados:

- Áudio captado pelo microfone do seu dispositivo
- Gravações de áudio criadas por você com o Aplicativo
- Informações de contato, localização, fotos, dados da câmera ou identificadores de dispositivo
- Identificadores publicitários (IDFA, IDFV usados para rastreamento)
- Dados analíticos, telemetria de falhas encaminhada a serviços de terceiros, ou perfis comportamentais
- Dados de cartão de pagamento ou de cobrança (a Apple processa as compras — consulte o §7)

O HearRelay não contém quaisquer SDKs de terceiros para análises, publicidade ou rastreamento.

---

## 3. Dados processados localmente no seu dispositivo

O Aplicativo processa os seguintes dados no seu dispositivo, e **apenas no seu dispositivo**:

| Dado | Finalidade | Retenção |
|---|---|---|
| Áudio do microfone (ao vivo) | Monitoramento em tempo real para fones de ouvido ou para um dispositivo pareado na mesma rede Wi-Fi | Não armazenado |
| Gravações de áudio (opcional) | Você pode gravar sessões manualmente | Excluídas automaticamente após 24 horas, por padrão; você pode estender o prazo ou excluí-las antes |
| Histórico de conexão (nome do par, data da última conexão) | Recurso de conveniência para reconectar rapidamente | Armazenado localmente; removido ao desinstalar o Aplicativo |
| Preferências do Aplicativo (incluindo a data de início do período de avaliação para controle de compra) | Lembrar suas configurações | Armazenadas localmente |

Quando você desinstala o Aplicativo, todos os dados acima são removidos com ele.

---

## 4. Informações limitadas processadas pelo Apple iCloud (escopo da Apple ID)

Para permitir que seus próprios dispositivos Apple se encontrem na mesma rede Wi-Fi, o Aplicativo faz com que as seguintes informações limitadas de descoberta de dispositivo sejam armazenadas no **Apple iCloud Key-Value Storage**, dentro da sua conta Apple ID:

- Uma **chave pública** criptográfica gerada no seu dispositivo
- Uma **impressão digital SHA-256** dessa chave pública
- O **nome** do seu dispositivo (conforme definido em Ajustes do iOS → Geral → Sobre → Nome)
- A **plataforma**, o **modelo** do seu dispositivo, e a **versão do aplicativo** instalada
- A **data de criação** e a **data da última rotação** da chave

Essas informações são armazenadas no escopo da sua própria Apple ID, dentro do serviço iCloud da Apple, e não são visíveis para outros titulares de Apple ID nem para a CONEX. A CONEX não opera o Apple iCloud e não acessa essas informações em seus próprios servidores. O tratamento pela Apple é regido pela política de privacidade da própria Apple e pelos termos do iCloud.

**Dependendo da lei aplicável e das configurações do nome do seu dispositivo, algumas dessas informações podem ser consideradas dados pessoais** — por exemplo, se o nome do seu dispositivo contiver seu nome completo. Descrevemo-las aqui por transparência. Você pode alterar o nome do seu dispositivo a qualquer momento nos Ajustes do iOS, e pode purgar a identidade do Aplicativo (girando sua chave e apagando a entrada) em **Ajustes → Segurança → Redefinir toda a segurança do dispositivo** dentro do Aplicativo.

---

## 5. Comunicação em rede

O HearRelay se comunica **apenas** com outros dispositivos Apple que estejam:

1. Conectados à **mesma Apple ID**, **e**
2. Conectados à **mesma rede Wi-Fi / rede local**

A comunicação é criptografada com o **HearRelay Secure Channel** (acordo de chaves X25519 ECDH + AEAD ChaCha20-Poly1305 com proteção contra repetição). O HearRelay **não** envia quaisquer dados pela Internet para servidores remotos, nem oferece suporte a monitoramento remoto entre redes. O uso remoto é deliberadamente proibido para evitar vigilância clandestina.

---

## 6. Gravações de áudio que você cria

Se você ativar o recurso de gravação:

- As gravações são salvas **apenas no dispositivo que as criou**
- As gravações são armazenadas dentro do sandbox do Aplicativo com **criptografia em nível de arquivo** (`NSFileProtectionComplete`)
- As gravações são **excluídas automaticamente 24 horas** após a criação, salvo se você escolher explicitamente preservá-las
- Você pode compartilhar ou exportar gravações por meio da folha de compartilhamento do iOS, sob seu controle
- As gravações nunca são enviadas pelo Aplicativo à CONEX nem a terceiros

Você é responsável por confirmar que qualquer gravação ou monitoramento ao vivo que realize cumpra todas as leis aplicáveis — incluindo exigências de consentimento que possam aplicar-se ao seu local. Consulte nossos [Termos de Uso](/pt-BR/terms/) e a página de [Suporte](/pt-BR/support/) para mais informações.

---

## 7. Terceiros, pagamentos e a App Store

- A CONEX **não** compartilha dados com terceiros.
- O Aplicativo **não** utiliza SDKs de publicidade, análises ou perfilamento.
- A CONEX **não** vende nem aluga dados de qualquer espécie.

A distribuição e os pagamentos são realizados pela Apple por meio da App Store e da Compra no Aplicativo (In-App Purchase). **O HearRelay Full Access é uma compra única, do tipo Não-Consumível, e não uma assinatura com renovação automática.** Preços, impostos, reembolsos e cobranças são processados pela Apple sob os Termos da App Store e dos Apple Media Services. A CONEX não recebe números de cartão de pagamento nem detalhes de cobrança. Você pode restaurar uma compra anterior usando a opção **Restore Purchases** dentro do Aplicativo.

Quando a Apple processa sua compra ou entrega atualizações, a política de privacidade da própria Apple se aplica a essa atividade. Quaisquer informações de diagnóstico que a Apple coletar do seu dispositivo (por exemplo, registros de falhas enviados via "Compartilhar com Desenvolvedores de Apps") são regidas pelos Ajustes do iOS e pelos termos para desenvolvedores da Apple.

---

## 8. Nosso site

O site do HearRelay em <https://hearrelay.app/> é um site informacional estático hospedado no GitHub Pages. **Não** utilizamos cookies publicitários, cookies analíticos, pixels de rastreamento ou tags de marketing de terceiros. Caso isso mude, atualizaremos esta Política e forneceremos quaisquer avisos ou opções exigidos pela lei aplicável.

---

## 9. Usuários internacionais

Como o HearRelay não transfere dados dos seus dispositivos para servidores da CONEX, não há transferência internacional de dados pessoais realizada pela CONEX.

### 9.1 Usuários no Espaço Econômico Europeu (EEE), Reino Unido e Suíça

O Aplicativo é projetado de modo que a CONEX não colete nem receba em seus próprios servidores áudio, gravações, informações de pagamento, dados analíticos, identificadores publicitários ou dados de rastreamento.

Informações limitadas de descoberta de dispositivo podem ser armazenadas no Apple iCloud, dentro da sua conta Apple ID (§4). A CONEX não opera o Apple iCloud e não acessa essas informações em seus próprios servidores. Quando a lei aplicável tratar tais informações como dados pessoais, as **finalidades** de qualquer processamento se limitam a permitir descoberta de dispositivos, autenticação mútua, segurança e comunicação local ponto-a-ponto entre seus próprios dispositivos; a **base legal** é o seu consentimento para usar o Aplicativo para essa finalidade, e o seu legítimo interesse em conectar privadamente os seus próprios dispositivos.

A CONEX avaliou a exigência prevista no Artigo 27 do GDPR de designar um representante na União Europeia e concluiu que a natureza limitada, ocasional e de baixo risco de qualquer processamento se enquadra na isenção do Artigo 27(2)(a). Essa determinação está documentada internamente e é revisada quando fatos relevantes mudam. Se você for uma autoridade de supervisão ou um titular de dados no EEE que precise nos contatar, utilize **hearrelay-privacy@conex-cp.com** — comprometemo-nos a responder dentro dos prazos legais.

### 9.2 Usuários no Brasil

A postura de tratamento do Aplicativo sob a LGPD (Lei 13.709/2018) reflete o §9.1. A CONEX não tem ciência de quaisquer dados pessoais processados em seus próprios servidores. A CONEX não nomeou um Encarregado (DPO) local com base no fato de que não ocorre nenhum tratamento de dados pessoais em larga escala ou de alto risco por parte da CONEX. O contato acima serve como ponto de contato para solicitações relativas à LGPD.

### 9.3 Usuários no Japão

A CONEX não inclui SDKs de publicidade, análise ou rastreamento de terceiros no Aplicativo, e não transmite informações relacionadas a usuários para seus próprios servidores. O Apple iCloud Key-Value Storage é usado exclusivamente para sincronizar as informações limitadas de descoberta de dispositivo descritas no §4 dentro da sua própria conta Apple ID; a CONEX não recebe essas informações em seus próprios servidores. Referimo-nos a essa configuração de boa-fé ao avaliar o regime japonês de notificação de transmissão externa previsto na Lei de Negócios de Telecomunicações.

### 9.4 Usuários em Hong Kong / Taiwan

A mesma postura de tratamento se aplica. A CONEX está ciente de que a PDPO (Hong Kong) e a Lei de Proteção de Informações Pessoais (Taiwan) definem dados pessoais e informações pessoais de forma ampla; consulte os §4 e §10 para nossa posição e os direitos que você pode exercer.

---

## 10. Privacidade de crianças

O HearRelay é um utilitário destinado a adultos, normalmente pais ou responsáveis. **Não é direcionado a crianças menores de 13 anos**, e a CONEX não coleta intencionalmente dados pessoais de crianças. O processamento do Aplicativo ocorre localmente no seu dispositivo, portanto nenhum dado pessoal de crianças é coletado, armazenado ou transmitido à CONEX.

---

## 11. Seus direitos

Como a CONEX não mantém dados pessoais sobre você em seus servidores, normalmente não há nada para acessar, corrigir, excluir, exportar ou restringir. Ainda assim, dependendo da sua localização (EEE, Reino Unido, Califórnia, Brasil, Japão, Hong Kong, Taiwan etc.), você pode ter direitos legais, incluindo:

- Direito de acesso
- Direito à retificação
- Direito à exclusão
- Direito de se opor ou de restringir o tratamento
- Direito à portabilidade dos dados
- Direito de optar por não ser objeto de "venda" ou "compartilhamento" — a CONEX não vende nem compartilha dados pessoais
- Direito de apresentar reclamação à autoridade de supervisão local

Para exercer qualquer direito, entre em contato em **hearrelay-privacy@conex-cp.com**. Observe que, para excluir todos os dados que o Aplicativo armazenou localmente, basta desinstalar o Aplicativo do seu dispositivo. Para purgar a identidade por dispositivo do Aplicativo no Apple iCloud (§4), use **Ajustes → Segurança → Redefinir toda a segurança do dispositivo** dentro do Aplicativo.

---

## 12. Segurança

Utilizamos proteções de padrão da indústria:

- **HearRelay Secure Channel** (X25519 ECDH + AEAD ChaCha20-Poly1305) para toda a comunicação dispositivo-a-dispositivo
- Chaves de identidade **P-256** geradas e armazenadas no **Secure Enclave** quando disponível, com fallback no Keychain
- **Fixação de chave pública (public-key pinning)** por meio de uma lista de confiança no escopo do iCloud, para impedir que dispositivos impostores se conectem
- **Proteção de arquivos** (`NSFileProtectionComplete`) para gravações locais

Nenhum método de transmissão ou armazenamento é perfeitamente seguro. Para relatar uma vulnerabilidade, consulte nossa [página de Segurança](/pt-BR/security/) e envie um e-mail para **hearrelay-security@conex-cp.com**.

---

## 13. Alterações a esta política

Podemos revisar esta Política de Privacidade. A data da revisão será atualizada no topo desta página, e alterações materiais serão anunciadas nas notas de versão do Aplicativo. Quando a lei aplicável exigir, obteremos seu consentimento ou forneceremos um aviso prévio razoável e uma oportunidade significativa para você deixar de usar o Aplicativo antes que a alteração entre em vigor.

---

## 14. Contato

- Privacidade: **hearrelay-privacy@conex-cp.com**
- Suporte: **hearrelay-support@conex-cp.com**
- Segurança: **hearrelay-security@conex-cp.com**
- Web: <https://hearrelay.app/>

---

**Traduções disponíveis em:** [日本語](/ja/privacy/) · [Français](/fr/privacy/) · [Español](/es/privacy/) · [Português (Brasil)](/pt-BR/privacy/) · [简体中文](/zh-Hans/privacy/)

Quando esta Política for fornecida em qualquer idioma diferente do inglês, a **versão em inglês prevalecerá** na medida permitida pela lei aplicável. Esta regra de precedência não limita os direitos que lhe são conferidos por leis imperativas de proteção ao consumidor, privacidade ou proteção de dados do seu país ou região.
