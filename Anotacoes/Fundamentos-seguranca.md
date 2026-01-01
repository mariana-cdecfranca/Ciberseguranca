# Ciberseguraça: fundamentos e práticas integradas
## Fundamentos da segurança da informação 

### Terminologias de segurança
- dados = átomos da informação
   - ativo (valor para a organzação)
 
- segurança deve estar em equilíbrio entre Funcionalidade, Segurança e Usabilidade
- princípios:
   - **confidencialidade:** acesso somente para a autorizados; restrição de acesso
      - ex: uso de MFA
    
   - **integridade:** informações completas, sem alterações (alterações somente por autorizados)
      - ex: banco de dados, logs...
    
   - **disponibilidade:** acesso garantido à autorizados
   - **autenticidade:** garante que a informação é real e confiável, abrangendo conceito de **não repúdio**
      - ex: uso de assinatura digital
      - **princípio de não repúdio** garante que o autor não negue a sua ação
    
   - **auditoria:** garante quem fez o quê, quando e onde
      - ex: logs que registram ações e eventos
    
   - **responsabilidade (accountability):** permite identificar quem realizou ações no sistema
 
- outros conceitos:
   - **controle de segurança:** contramedidas para previnir ou reagir a ameaças
   -  **mecanismos de segurança:** estrutura defensiva de proteção
   -  **políticas de segurança:** conjunto de regras e regulamentações de segurança
   -  **vulnerabilidades:** falhas/lacunas em sistemas, processos ou pessoas
       - ex: senhas fracas, softwares desatualizados
    

### Terminologias de ameaças
   -  **ameaças:** podem explorar vulnerabilidades e causar danos ao ambiente e à aplicação
       - ameaça = potencial ataque
       - ex: malwares, worms, cavalo de Troia, keylogger, phishing, DDOS...
          - malwares: software malicioso projetado para projetar dano
              - ex: vírus, cavalo de Troia, bot, worms, etc
           
          - engenharia social: indivíduos são enganados e levados a revelar informações ou realizar ações arriscadas
          - phishing: forma de engenharia social que usa comunicação eletrônica
             - ex: e-mail
           
   -  **risco:** potencial perda indesejada e inesperada que pode resultar de uma determinada ação
       - risco = ameaça * impacto
       - podemos:
          - aceitar (conviver com o risco; risco baixo ou custo maior que o impacto)
          - mitigar (reduzir impacto, implementação de controles técnicos/administrativos)
          - transferir (para empresa terceira, por exemplo; responsabilidade legal ou financeira é transferida)
          - evitar (remover/corrigit vulnerabilidade)
        
   -  **exploit:** quando atacante consegue tirar proveito de uma vulnerabilidade
        
### CVE, CWE e CVSS
- **CVE (Common Vulnerabilities and Exposures):**
   - é um identificador único para uma vulnerabilidade conhecida
   - serve para todo o mundo falar da mesma falha, identificando e categorizando vulnerabilidades
   - mantido pelo MITRE (CVE.org)
      - fornece informações sobre software afetado, sobre a falha e descrição resumida
   - formato: CVE-AAAAA-NNNNNN
      - ex: CVE-2025-12345
    
- **CWE (Common Weakness Enumeration):**
 - descreve tipos de falhas comuns em sistemas
 - usado para análise, prevenção e ensino
 - mantido pelo MITRE (CWE.mitre.org)
    - ex:
        - CWE-79: Cross-Site Scripting (XSS)
        - CWE-89: SQL Injection
      
 - **CVSS (Common Vulnerability Scoring System):**
  - mede o impacto e a facilidade de exploração da vulnerabilidade através de sistema de pontuação (0-10)
  - usado para priorizar correções
    
| Pontuação  | Severidade |
| ---------- | ---------- |
| 0.0        | Nenhuma    |
| 0.1 – 3.9  | Baixa      |
| 4.0 – 6.9  | Média      |
| 7.0 – 8.9  | Alta       |
| 9.0 – 10.0 | Crítica    |

### Ameaças e agentes maliciosos
- um ataque está sempre relacionado a: motivo (interesse no valor do sistema alvo), método (técnicas para explorar falhas) e vulnerabilidade
- vetor de ataque: caminho percorrido pelo atacante para explorar vulnerabilidade (ex: anexos de e-mail, salas de bate-papo)
- ameaças e vetores:
   - **APT (Advanced Persistent Threats):** fico em roubar informações da vítima sem ela saber
   - **vírus ou worms:** principais ameaças nas redes, capaz de infectar toda a rede em segundos
   - **ransomware:** restringem acesso de um arquivo/pasta, exigindo pagamento para liberação
   - **ameaças mobile:** foco em ataque mobile, que possuem menos controles de segurança
   - **botnet:** larga rede de sistemas infectados usados para promover mais ataques
   - **insider attack:** ataque realizado em uma rede corporativa por uma pessoa confiável autorizada
   - **phishing:** envio de e-mail falso para tentar adquirir uma conta
   - **ameaças web:** roubo de senhas, envio de phishing ou aquisição de informação privada para prejudicar a segurança
   - **ameaças IoT:** usam acesso em dispositivos remotos e permitem diversos ataques remotos
   - **sistema operacional:** ataque a vulnerabilidades no S.O, instalação, design ou configuração
   - **microconfiguration attack:** afetam servidores web, plataformas, base de dados, rede ou framework, que pode resultar em acesso ilegal ao sistema
  
