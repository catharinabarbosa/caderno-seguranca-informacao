🛡️ Caderno Temático: Fundamentos de Segurança da Informação e Boas Práticas de Proteção de Dados
Projeto desenvolvido para o desafio da DIO (Digital Innovation One) — uso da Inteligência Artificial (NotebookLM) como ferramenta de aprendizagem ativa.


🎯 Contexto e Objetivos
Assunto escolhido: Segurança da Informação, com foco em fundamentos técnicos (confidencialidade, integridade, disponibilidade), boas práticas de proteção de dados e noções introdutórias de conformidade (LGPD).

Por que esse tema? Segurança da Informação é uma área transversal a toda a tecnologia — independente da trilha (dev, dados, infra), entender os princípios básicos de proteção de dados e riscos é essencial para atuar no mercado de forma responsável.

Objetivos de estudo:

Compreender os pilares da Segurança da Informação (CID: Confidencialidade, Integridade, Disponibilidade);
Entender os principais tipos de ameaças e vulnerabilidades mais comuns (ex: phishing, engenharia social, injeção de código);
Conhecer boas práticas de proteção de dados pessoais e sua relação com a LGPD;
Construir um vocabulário técnico sólido sobre o tema para uso profissional e em entrevistas.


📚 Curadoria de Fontes
Fontes abertas selecionadas e carregadas no NotebookLM:

#
Fonte
Tipo
Link
1
Cartilha de Segurança para Internet — CERT.br
PDF
https://cartilha.cert.br/livro/cartilha-seguranca-internet.pdf
2
OWASP Top 10 (2021)
Web
https://owasp.org/Top10/2021/
3
NIST Cybersecurity Framework (CSF) 2.0
PDF
https://nvlpubs.nist.gov/nistpubs/CSWP/NIST.CSWP.29.pdf
4
Lei Geral de Proteção de Dados (Lei nº 13.709/2018)
PDF (texto oficial — Senado Federal)
https://www2.senado.leg.br/bdsf/bitstream/handle/id/658231/Lei_geral_protecao_dados_pessoais_1ed.pdf



🧠 Engenharia de Prompts e "Cicatrizes"
Aqui documento as perguntas estratégicas feitas ao NotebookLM, as respostas obtidas e as dificuldades encontradas no processo (troubleshooting).
Prompt 1
Pergunta: "Com base nas fontes carregadas, quais são os três pilares da Segurança da Informação e como cada um se aplica a um cenário prático de e-commerce?"

Resposta obtida (resumo): O NotebookLM identificou os três pilares clássicos — Confidencialidade, Integridade e Disponibilidade — e aplicou cada um a um cenário de e-commerce: Confidencialidade via HTTPS/criptografia na hora de coletar dados de cartão e senha; Integridade via assinaturas digitais e protocolos que impedem alteração dos dados de um pedido (valor, endereço) em trânsito; Disponibilidade relacionada à necessidade da loja virtual estar sempre online, citando ataques DoS/DDoS como ameaça direta a esse pilar. A IA ainda complementou de forma proativa, citando autenticação e não repúdio como requisitos adicionais mencionados nas fontes mais recentes.

Referência usada pela IA: Cartilha de Segurança para Internet (CERT.br) — conceito de sistema seguro (CID) e seção sobre ameaças/DoS.

Dificuldade encontrada: Nenhuma reformulação foi necessária — a resposta já veio estruturada e com exemplos práticos de e-commerce de primeira, sem precisar de ajustes. O prompt original já pedia especificamente por um "cenário prático", o que evitou uma resposta genérica.


Prompt 2
Pergunta: "Quais são as principais diferenças entre os controles técnicos sugeridos pelo NIST Cybersecurity Framework e as exigências de conformidade da LGPD? Traga exemplos práticos de como uma empresa poderia atender aos dois ao mesmo tempo."

Resposta obtida (resumo): A IA foi transparente ao apontar que o NIST CSF não estava detalhado nas fontes carregadas, então tratou-o como "informação externa" e não misturou isso com o conteúdo real da LGPD — o que é um bom sinal de rigor. Traçou diferenças claras: a LGPD é lei obrigatória focada em princípios (finalidade, necessidade, transparência) e prevê sanções (multas de até 2% do faturamento, limitadas a R$ 50 milhões), enquanto o NIST é um framework voluntário, mais técnico, organizado em funções (Identificar, Proteger, Detectar, Responder, Recuperar). Trouxe exemplos práticos de atendimento conjunto: criptografia (confidencialidade), gestão de acessos com autenticação em duas etapas e privilégio mínimo, monitoramento/logs (ligado ao princípio de responsabilização da LGPD e à função "Detectar" do NIST) e gestão de vulnerabilidades/patches.

Referência usada pela IA: Lei nº 13.709/2018 (LGPD) para os pontos legais; conhecimento geral (não das fontes) para os detalhes técnicos do NIST CSF.

Dificuldade encontrada: A própria IA sinalizou a limitação — como o NIST CSF não estava entre as fontes carregadas, ela deixou explícito quando estava usando "informação externa" em vez de citar as fontes. Isso reforça a importância de, se o objetivo é uma resposta 100% baseada em fontes, carregar o PDF oficial do NIST CSF no notebook antes de repetir esse prompt.


Prompt 3
Pergunta: "Crie um glossário com os 10 termos mais importantes sobre segurança da informação presentes nas fontes, com uma definição de até 2 linhas para cada termo."

Resposta obtida (resumo): Gerou um glossário limpo com 10 termos técnicos relevantes e bem distribuídos entre conceitos fundamentais (Confidencialidade, Integridade, Disponibilidade), ameaças (Malware, Phishing, Vulnerabilidade), mecanismos de proteção (Criptografia, Autenticação, Backup) e o marco legal (LGPD) — sem repetições ou termos genéricos demais.

Dificuldade encontrada: Nenhuma — o resultado já veio direto ao ponto e bem equilibrado entre os temas das fontes, sem necessidade de refinamento.



💡 Dica de ouro seguida: para cada prompt, além da resposta, registrei a fonte usada pela IA e as dificuldades de obter a melhor resposta — isso mostra o raciocínio por trás do resultado final. Vale destacar que o Prompt 2 revelou um comportamento importante do NotebookLM: quando não tem a fonte carregada, ele avisa e separa claramente o que é "conhecimento externo" do que vem dos documentos — isso é um ótimo ponto de aprendizado sobre confiabilidade de IA.


📖 Miniguia de Estudo (Entrega Final)
🔹 Resumos Estruturados
1. Pilares da Segurança da Informação (CID) Um sistema é considerado seguro quando atende a três requisitos básicos:

Confidencialidade: garantir que a informação esteja disponível apenas para quem é autorizado. Ex: HTTPS e criptografia protegendo dados de cartão de crédito em um checkout de e-commerce.
Integridade: garantir que a informação não seja alterada indevidamente. Ex: assinaturas digitais impedindo que um atacante altere o valor ou endereço de um pedido em trânsito.
Disponibilidade: garantir que os serviços estejam acessíveis quando necessário. Ex: uma loja virtual precisa estar sempre online — ataques DoS/DDoS visam justamente quebrar esse pilar.

Além dos três pilares clássicos, fontes mais recentes também citam autenticação (confirmar que a entidade é quem diz ser) e não repúdio (impedir que alguém negue ter realizado uma ação) como requisitos complementares no ambiente digital.

2. Principais Ameaças

Phishing e engenharia social;
Malware (vírus, ransomware, spyware, bots);
Ataques de Negação de Serviço (DoS/DDoS), que comprometem diretamente a disponibilidade.

3. LGPD x NIST Cybersecurity Framework São abordagens complementares, não concorrentes:

LGPD: lei obrigatória, focada em princípios (finalidade, necessidade, transparência) e com sanções previstas (multas de até 2% do faturamento, limitadas a R$ 50 milhões por infração).
NIST CSF: framework voluntário e mais técnico, organizado em 5 funções (Identificar, Proteger, Detectar, Responder, Recuperar) — não substitui a lei, mas ajuda a operacionalizar tecnicamente o que a LGPD exige em termos de "medidas técnicas e administrativas".
Exemplos de atendimento conjunto: criptografia de dados (confidencialidade), gestão de acessos com autenticação em duas etapas e privilégio mínimo, monitoramento e logs (responsabilização), e gestão de vulnerabilidades/patches (prevenção).


🔹 Glossário
Termo
Definição
Confidencialidade
Garante que a informação esteja disponível apenas para quem é devidamente autorizado, protegendo-a contra acesso de terceiros
Integridade
Assegura que a informação não seja destruída ou corrompida indevidamente, mantendo a exatidão dos dados originais
Disponibilidade
Garante que os serviços e recursos do sistema estejam acessíveis sempre que forem necessários pelos usuários autorizados
Criptografia
Ciência de escrever mensagens em forma cifrada, tornando-as ilegíveis para quem não possui a chave de decodificação
LGPD
Lei Geral de Proteção de Dados — legislação brasileira que regula o tratamento de dados pessoais para proteger a privacidade dos cidadãos
Malware (Código Malicioso)
Termo genérico para programas desenvolvidos para executar ações danosas em um computador, como vírus e bots
Phishing
Fraude que tenta obter dados pessoais e financeiros através de mensagens enganosas que se passam por instituições conhecidas
Autenticação
Processo que verifica a identidade de uma entidade (pessoa ou sistema), assegurando que ela é realmente quem diz ser
Vulnerabilidade
Falha no projeto, implementação ou configuração de um sistema que pode ser explorada por atacantes
Backup (Cópia de Segurança)
Cópia de dados armazenada em local seguro para permitir recuperação em caso de falhas ou invasões



🔹 Prompts Reutilizáveis
Conjunto de prompts testados e validados, prontos para reutilização em futuras revisões do tema:

1. "Com base nas fontes carregadas, quais são os três pilares da Segurança da Informação e como cada um se aplica a um cenário prático de [substituir pelo setor: e-commerce, saúde, educação, etc.]?"

2. "Quais são as principais diferenças entre os controles técnicos sugeridos pelo NIST Cybersecurity Framework e as exigências de conformidade da LGPD? Traga exemplos práticos de como uma empresa poderia atender aos dois ao mesmo tempo."

3. "Crie um glossário com os 10 termos mais importantes sobre segurança da informação presentes nas fontes, com uma definição de até 2 linhas para cada termo."

4. "Como a LGPD define o princípio da segurança?"

5. "O que caracteriza um dado pessoal sensível na lei?"

6. "Quais sanções a ANPD pode aplicar em casos de infração?"

7. "Como funciona o relatório de impacto à proteção de dados?"

💡 Os prompts 4 a 7 surgiram como sugestões automáticas do próprio NotebookLM após as respostas dos Prompts 1 e 2 — vale a pena testá-los para aprofundar o tema em uma futura revisão.


🧩 Ferramentas Utilizadas
NotebookLM — curadoria e interrogação das fontes;
GitHub — versionamento e hospedagem do repositório;
Markdown — formatação da documentação.


✅ Conclusão
Este projeto demonstrou como a IA pode ser utilizada não apenas como fonte de respostas prontas, mas como uma ferramenta de aprendizagem ativa — exigindo curadoria crítica de fontes, formulação estratégica de perguntas e validação constante das respostas obtidas.



Desenvolvido como parte do desafio de projeto da Digital Innovation One (DIO).

