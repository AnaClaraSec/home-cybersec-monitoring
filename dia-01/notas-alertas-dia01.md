# Notas Alertas Dia01

**Data**: 28/06/2025  
**Ferramenta**: Wireshark e Nmap


## FILTRO HTTPS:
- Durante o filtro de tráfego HTTPS, foram detectadas requisições para o Google Cloud. No entanto, isso não representa nenhum risco ou perigo, já que é um tráfego legítimo para a infraestrutura do Google.

## FILTRO DNS:
- Durante o monitoramento de rede com Wireshark usando filtros DNS, notei uma requisição ao domínio **avast.com**. Por não possuir o software da Avast instalado, inicialmente suspeitei de atividade incomum. Após investigação, constatei que se trata de um comportamento benigno, possivelmente relacionado a serviços de terceiros ou mecanismos de reputação automática.

## FILTRO UDP:
- Ao analisar o tráfego UDP, não foram observadas comunicações incomuns ou tráfego inesperado. No entanto, algumas requisições DNS em **UDP** foram registradas, o que é esperado em uma rede doméstica, dado que o DNS geralmente utiliza o protocolo UDP para resolver nomes de domínio.

## FILTRO TCP:
- Durante a captura de pacotes TCP, observei algumas **tentativas de conexão** para a **porta 80 (HTTP)**. Não houve nenhum sinal de ataque ou tráfego malicioso, mas é importante observar que essas tentativas eram em horários irregulares. Em geral, o tráfego TCP parece estar dentro dos padrões normais para uma rede doméstica, sem qualquer comportamento suspeito.

### Alertas Observados:

 **Informativo**:
  - Foi observado tráfego DNS para o domínio **avast.com**. Após investigação, confirmou-se que o tráfego é benigno, possivelmente relacionado a **processos de verificação de reputação** e não representa risco de segurança.





