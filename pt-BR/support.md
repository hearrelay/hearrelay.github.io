---
title: Suporte — HearRelay
lang: pt-BR
---

# Suporte

Obrigado por usar o **HearRelay**. Esta página reúne dicas de solução de problemas e como entrar em contato.

> Esta tradução é fornecida por conveniência. Em caso de divergência com a [versão em inglês](/en/support/), prevalecerá a versão em inglês.

---

## Ajuda rápida

### "Nenhum dispositivo encontrado" ao tentar parear

Ambos os dispositivos devem:

1. Estar conectados com **a mesma Apple ID**
2. Estar conectados à **mesma rede Wi-Fi** (mesma sub-rede)
3. Estar com o **iCloud** ativado nos Ajustes do iOS
4. Ter concedido ao HearRelay as permissões de **Microfone** e **Rede Local**

Se ainda assim não vir o outro dispositivo, toque no botão de atualizar no seletor de pareamento ou reinicie o Aplicativo em ambos os dispositivos.

### O áudio trava ou tem cortes

- Aproxime-se do seu roteador Wi-Fi ou mude para uma rede de 5 GHz
- Fones Bluetooth com má recepção podem causar cortes — experimente cabeados ou outro par
- Tráfego de rede intenso (downloads grandes, videochamadas) na mesma Wi-Fi pode afetar o áudio em tempo real

### O som dos AirPods parece ter qualidade baixa no modo Standalone

O HearRelay restringe o microfone ao **microfone integrado** no modo Standalone para evitar forçar o Bluetooth a um modo de baixa largura de banda (HFP). Use o microfone integrado como entrada e os AirPods apenas como saída. Isso é intencional.

### A gravação não foi mantida

As gravações são excluídas automaticamente **24 horas após a criação**, a menos que você toque em **Preservar**. Uma vez preservadas, permanecem até que você as exclua.

### O HearRelay parou de gravar quando bloqueei a tela

O HearRelay continua a capturar e retransmitir áudio em segundo plano enquanto a tela está bloqueada. Se a captura parar:

- Certifique-se de que a **Atualização em Segundo Plano** esteja permitida para o HearRelay (Ajustes do iOS → Geral → Atualização em Segundo Plano)
- Certifique-se de que o **Modo de Baixo Consumo** não esteja suspendendo agressivamente tarefas em segundo plano
- Algumas versões do iOS suspendem sessões de áudio quando outro app de áudio assume — encerre esse outro app

### O ícone na Dynamic Island / Tela Bloqueada desapareceu

As Live Activities têm uma duração máxima imposta pelo sistema operacional (cerca de 8 horas). Depois disso, o indicador pode parar de atualizar mesmo com o HearRelay em funcionamento. Reabra o Aplicativo para atualizar.

---

## Lista de permissões

| Permissão | Necessária para | Caminho nos Ajustes |
|---|---|---|
| Microfone | Qualquer monitoramento | Ajustes → HearRelay → Microfone |
| Rede Local | Modo pareado (envio / recebimento com outros dispositivos) | Ajustes → HearRelay → Rede Local |
| iCloud (com sessão iniciada) | Modo pareado (descobrir seus outros dispositivos) | Ajustes → \[Seu nome\] → iCloud |
| Atualização em Segundo Plano | Monitoramento contínuo com a tela desligada | Ajustes → Geral → Atualização em Segundo Plano |

Se Rede Local ou iCloud não estiverem disponíveis, você ainda pode usar o modo **Standalone**.

---

## Contato

- **E-mail:** hearrelay-support@conex-cp.com
- Buscamos responder em poucos dias úteis. Inclua a versão do iOS, o modelo do dispositivo e uma descrição dos passos que você seguiu.

Para questões de privacidade, veja a [Política de Privacidade](/pt-BR/privacy/) ou envie e-mail para **hearrelay-privacy@conex-cp.com**.
Para relatos de segurança, veja a [página de Segurança](/pt-BR/security/) ou envie e-mail para **hearrelay-security@conex-cp.com**.

---

**English version:** [Support](/en/support/)
