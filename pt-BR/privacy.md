---
title: Política de Privacidade — HearRelay
lang: pt-BR
---

# Política de Privacidade

**Data de vigência: 24 de abril de 2026**
**Última atualização: 24 de abril de 2026**

> Esta tradução é fornecida por conveniência. Em caso de divergência entre esta tradução e a [versão em inglês](/en/privacy/), prevalecerá a versão em inglês.

O HearRelay (o "Aplicativo") foi projetado para ser privado por padrão. Esta política explica quais dados são, e não são, processados quando você usa o HearRelay.

Se tiver alguma dúvida, entre em contato conosco pelo e-mail **hearrelay-privacy@conex-cp.com**.

---

## 1. Quem somos

O HearRelay é desenvolvido pela **CONEX Corporation** (株式会社CONEX), uma empresa constituída no Japão (o "Desenvolvedor", "nós"). Como o HearRelay não processa dados pessoais em nossos servidores, não atuamos como "controlador de dados" em sentido substancial — somos o publicador do aplicativo. Para correspondência, utilize os endereços de e-mail no final desta página.

---

## 2. Dados que não coletamos

**Não** coletamos, armazenamos, transmitimos aos nossos servidores nem compartilhamos nenhum dos seguintes dados:

- Áudio captado pelo microfone do seu dispositivo
- Gravações de áudio criadas por você com o Aplicativo
- Informações de contato, localização, fotos, dados da câmera ou identificadores de dispositivo
- Identificadores publicitários (IDFA, IDFV usados para rastreamento)
- Análises, telemetria de falhas enviada a serviços de terceiros, ou perfis comportamentais

O HearRelay não contém quaisquer SDKs de terceiros para análises, publicidade ou rastreamento.

---

## 3. Dados processados localmente no seu dispositivo

O Aplicativo processa os seguintes dados no seu dispositivo, e **apenas no seu dispositivo**:

| Dado | Finalidade | Retenção |
|---|---|---|
| Áudio do microfone (ao vivo) | Monitoramento em tempo real para fones de ouvido ou dispositivo pareado na mesma rede Wi-Fi | Não armazenado |
| Gravações de áudio (opcional) | Você pode gravar sessões manualmente | Excluídas automaticamente após 24 horas por padrão; você pode estender ou excluir antes |
| Histórico de conexão (nome do par, última conexão) | Recurso de conveniência para reconectar rapidamente | Armazenado localmente; removido ao desinstalar o Aplicativo |
| Preferências do aplicativo | Lembrar suas configurações | Armazenadas localmente |

Quando você desinstala o Aplicativo, todos os dados acima são removidos com ele.

---

## 4. Dados tratados brevemente pela infraestrutura da Apple

Para permitir que seus próprios dispositivos Apple se encontrem na mesma rede Wi-Fi, o HearRelay utiliza o **iCloud Key-Value Storage**, fornecido pela Apple, para publicar:

- Uma **chave pública** criptográfica gerada no seu dispositivo
- Uma **impressão digital** (SHA-256) dessa chave
- O **nome**, **plataforma**, **modelo** do seu dispositivo, e a **versão do aplicativo**

Esses dados são armazenados no escopo da sua própria Apple ID, dentro do serviço iCloud da Apple, e não são visíveis para outros titulares de Apple ID nem para nós. O Desenvolvedor não opera servidores e não tem acesso a esses dados. O tratamento pela Apple é regido pela política de privacidade da própria Apple.

---

## 5. Comunicação em rede

O HearRelay se comunica **apenas** com outros dispositivos Apple que estejam:

1. Conectados à **mesma Apple ID**, **e**
2. Na **mesma rede Wi-Fi / rede local**

A comunicação é criptografada com **TLS 1.3**. O HearRelay **não** envia quaisquer dados pela Internet para servidores remotos, nem oferece suporte a monitoramento remoto entre redes. O uso remoto é deliberadamente proibido para evitar vigilância clandestina.

---

## 6. Gravações que você cria

Se você ativar o recurso de gravação:

- As gravações são salvas **apenas no dispositivo que as criou**
- São armazenadas dentro do sandbox do Aplicativo com **criptografia em nível de arquivo** (`NSFileProtectionComplete`)
- São **excluídas automaticamente 24 horas** após a criação, a menos que você escolha explicitamente preservá-las
- Você pode compartilhar ou exportar gravações pela folha de compartilhamento do iOS, sob seu controle
- As gravações nunca são enviadas a nós ou a terceiros pelo Aplicativo

---

## 7. Terceiros

- **Não** compartilhamos dados com terceiros.
- **Não** utilizamos SDKs de publicidade, análises ou perfilamento.
- **Não** vendemos nem alugamos dados de qualquer tipo.

A distribuição e o pagamento são realizados pela Apple por meio da App Store, sob os termos da própria Apple. Quando a Apple processa sua compra ou entrega atualizações, a política de privacidade da Apple se aplica a essa atividade.

---

## 8. Usuários internacionais

Como o HearRelay não transfere dados para fora dos seus dispositivos, não há transferência internacional de dados pessoais realizada por nós.

---

## 9. Privacidade de crianças

O HearRelay é um utilitário destinado a adultos, normalmente pais ou responsáveis. **Não é direcionado a crianças menores de 13 anos**, e não coletamos intencionalmente dados pessoais de crianças. O processamento do Aplicativo ocorre localmente no seu dispositivo, portanto nenhum dado pessoal de crianças é coletado, armazenado ou transmitido.

---

## 10. Seus direitos

Como não mantemos dados pessoais sobre você, normalmente não há nada a acessar, corrigir, excluir, exportar ou restringir. No entanto, dependendo da sua localização (EEE, Reino Unido, Califórnia, Brasil, Japão etc.), você pode ter direitos legais, incluindo os previstos na Lei Geral de Proteção de Dados Pessoais (LGPD) brasileira:

- Direito de acesso / confirmação do tratamento
- Direito à correção
- Direito à eliminação
- Direito de se opor ou restringir o tratamento
- Direito à portabilidade dos dados
- Direito de apresentar reclamação à ANPD ou à autoridade supervisora local

Para exercer qualquer direito, entre em contato em **hearrelay-privacy@conex-cp.com**. Para excluir todos os dados armazenados localmente pelo Aplicativo, basta desinstalar o Aplicativo do seu dispositivo.

---

## 11. Segurança

Utilizamos proteções de padrão da indústria:

- **TLS 1.3** para toda a comunicação entre dispositivos
- Chaves **Curve25519 / P-256** geradas e armazenadas no **Secure Enclave** quando disponível
- **Fixação de chave pública** para impedir que dispositivos impostores se conectem
- **Proteção de arquivos** (`NSFileProtectionComplete`) para gravações locais

Nenhum método de transmissão ou armazenamento é perfeitamente seguro. Para relatar uma vulnerabilidade, consulte nossa [página de segurança](/pt-BR/security/) e envie um e-mail para **hearrelay-security@conex-cp.com**.

---

## 12. Alterações a esta política

Podemos revisar esta Política de Privacidade. A data de revisão será atualizada no topo desta página, e alterações relevantes serão anunciadas nas notas de versão do Aplicativo. Continuar usando o Aplicativo após a entrada em vigor das alterações constitui aceitação.

---

## 13. Contato

- Privacidade: **hearrelay-privacy@conex-cp.com**
- Suporte: **hearrelay-support@conex-cp.com**
- Segurança: **hearrelay-security@conex-cp.com**
- Web: <https://hearrelay.app/>

---

**English version:** [Privacy Policy](/en/privacy/)
