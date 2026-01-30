# SOC-AS-A-SERVER

🧩 Micro-Desafios — SOC as a Server (1 VM + Docker)

Cada desafio leva 30–90 minutos, gera evidência e evolui o projeto.

🟢 Desafio 01 — SOC de Pé (Base)
🎯 Objetivo

Ter o SOC “vivo”.

🔧 Tarefas

Subir a VM SOC

Instalar Docker e Docker Compose

Subir Wazuh (stack completa)

✅ Sucesso

Dashboard acessível

Containers saudáveis

📌 Evidência

Print do docker ps

Print do dashboard

🟢 Desafio 02 — Primeiro Log
🎯 Objetivo

Confirmar coleta de logs.

🔧 Tarefas

Criar VM Linux (endpoint)

Instalar agente Wazuh

Validar comunicação

🧪 Teste
ssh usuario@endpoint

📌 Evidência

Log aparecendo no Wazuh

Host registrado

🟢 Desafio 03 — Login Suspeito
🎯 Objetivo

Entender alertas de autenticação.

🔧 Tarefas

Errar senha SSH várias vezes

Identificar alerta

Ler log bruto

📌 Evidência

Alerta disparado

Análise escrita (3–5 linhas)

🟡 Desafio 04 — Brute Force Controlado
🎯 Objetivo

Detectar ataque real.

🔧 Tarefas

Executar brute force leve

Identificar IP atacante

Classificar severidade

🧪 Ataque
hydra -l root -P small.txt ssh://IP

📌 Evidência

Alerta correlacionado

IP atacante identificado

🟡 Desafio 05 — Falso Positivo
🎯 Objetivo

Pensar como SOC N1.

🔧 Tarefas

Gerar alerta benigno

Decidir se é incidente

Justificar decisão

📌 Evidência

Registro “False Positive”

Motivo documentado

🟡 Desafio 06 — Integridade de Arquivo (FIM)
🎯 Objetivo

Detectar alteração crítica.

🔧 Tarefas

Alterar arquivo monitorado

Analisar hash

Ler regra FIM

🧪 Teste
touch /etc/teste_soc

📌 Evidência

Alerta FIM

Hash exibido

🟠 Desafio 07 — Incidente Manual (TheHive)
🎯 Objetivo

Trabalhar processo.

🔧 Tarefas

Subir TheHive

Criar incidente manual

Classificar TLP e severidade

📌 Evidência

Caso criado

Timeline preenchida

🟠 Desafio 08 — Automação Básica (Shuffle)
🎯 Objetivo

Introdução ao SOAR.

🔧 Tarefas

Subir Shuffle

Criar playbook simples

Notificar incidente

📌 Evidência

Print do workflow

Execução OK

🔴 Desafio 09 — IOC Malicioso
🎯 Objetivo

Threat Intelligence.

🔧 Tarefas

Subir MISP (opcional)

Importar IOC

Correlacionar evento

📌 Evidência

Alerta enriquecido

IOC identificado

🔴 Desafio 10 — Incidente Completo
🎯 Objetivo

Simular SOC real.

🔧 Tarefas

Ataque

Detecção

Investigação

Resposta

Documentação

📌 Entrega Final

Relatório completo

Lições aprendidas
