# Usuario-Windows-a-Analista-de-Ciberseguranca-via-Active-Directory
O Active Directory é o serviço de diretório da Microsoft que centraliza a administração de toda a infraestrutura. Ele funciona como o "cérebro" da rede, coordenando identidades, autenticação e permissões para todos os dispositivos no domínio.

1. Visão Geral: O "Cérebro" da Rede
Para quem inicia como usuário Windows, entender o AD é o primeiro grande degrau para sair de uma visão de máquinas isoladas para um ambiente corporativo gerenciado.
2. A Evolução da Rede e Centralização
A transição para o Active Directory marca a maturidade da TI em uma empresa.
•	Antes do AD (Máquinas Isoladas): Cada computador possui seus próprios usuários, senhas e permissões locais. A administração é manual e não escala.
•	Depois do AD (Gerenciamento Centralizado): Todos os computadores pertencem ao mesmo domínio e obedecem às mesmas Políticas de Grupo (GPO).
Principais Componentes:
•	Domínio (Domain): A unidade principal de administração (ex: empresa.local).
•	Controlador de Domínio (DC): O servidor que mantém o banco de dados do AD e valida identidades.
•	Unidades Organizacionais (OUs): Servem para organizar objetos (usuários, computadores) por departamentos.
•	Objetos: Tudo dentro do AD é um objeto com atributos (nome, login, e-mail).
3. Active Directory sob a Ótica da Segurança Digital
O AD não é uma ferramenta de segurança por si só, mas fornece a base sobre a qual as práticas de segurança são construídas.
•	Autenticação Segura: Utiliza protocolos como Kerberos, que emite tickets (TGT) para evitar o envio repetido de senhas na rede.
•	Controle de Acesso: Permissões são definidas por grupos, facilitando a auditoria de "quem pode acessar o quê".
•	Visibilidade: Todos os eventos de autenticação ficam registrados, criando uma base para monitorar atividades suspeitas.
O AD na Segurança Ofensiva:
Para um invasor, o AD é o alvo principal. Se um atacante obtém privilégios elevados no AD, ele pode controlar toda a organização. Conceitos fundamentais de ataque incluem:
•	Movimentação Lateral: Usar credenciais de uma máquina comprometida para acessar outros sistemas.
•	Escalonamento de Privilégios: Buscar contas com poderes de administrador de domínio.
4. Chegando ao SOC (Security Operations Center)
O SOC funciona como um centro de monitoramento onde analistas acompanham painéis de eventos de toda a infraestrutura.
•	O AD como Fonte de Dados: O AD é uma das principais fontes de informação para o SOC. Logs de logins malsucedidos, contas bloqueadas ou alterações de permissões são sinais críticos monitorados por ferramentas como SIEM (Gerenciamento de Informações e Eventos de Segurança).
•	Analogia da Cidade:
o	Active Directory: É a "Prefeitura" que mantém o cadastro de moradores e endereços.
o	SIEM: É o centro que recebe informações de câmeras e sensores de alarme.
o	SOC: É a equipe que trabalha nesse centro, interpreta os alertas e coordena a resposta a incidentes.
